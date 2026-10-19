# Mimari Taslak

**Durum:** İlk taslak. Mimari kararlar değiştikçe güncellenir.

## Hedef
Türkçe kullanım deneyimi sunan ve çok kiracılı yetkilendirme modeli içeren sanallaştırma yönetim platformu geliştirmek. İlk altyapı Proxmox VE'dir; ürün katmanının tamamı Proxmox'a özgü kavramlara bağlanmamalıdır.

## Mantıksal yapı
```text
Kullanıcı / Tarayıcı
        |
Türkçe Yönetim Arayüzü
        |
Ürün API'si ve Kimlik Doğrulama
        |
Yetkilendirme + Kiracı Kapsamı
        |
Uygulama Hizmetleri / Görev Takibi / Denetim Kayıtları
        |
Sanallaştırma Adaptörü
        |
Proxmox VE API'si
        |
Proxmox VE / KVM-QEMU / Depolama / Sanal Ağ
```

## Sorumluluk sınırları
- **Arayüz:** Türkçe metinler, formlar, durumlar ve kullanıcı etkileşimi.
- **Ürün API'si:** Ürüne ait kararlı API sözleşmesi; arayüz doğrudan Proxmox API'sine bağlanmaz.
- **Kimlik doğrulama/yetkilendirme:** Kullanıcı, rol, izin ve kiracı kapsamı; her istekte sunucu tarafında kontrol edilir.
- **Uygulama hizmetleri:** VM yaşam döngüsü, görev durumu, denetim kaydı ve doğrulama.
- **Sanallaştırma adaptörü:** Ürünün ortak işlemlerini seçilen altyapının API'sine dönüştürür.
- **Altyapı:** İlk sürümde Proxmox VE; altta KVM/QEMU ve Proxmox'un sağladığı depolama/ağ yönetimi.

## İlk soyutlanacak işlemler
- Sanal makine listeleme ve ayrıntı alma.
- Sanal makine oluşturma, başlatma, durdurma ve yeniden başlatma.
- Görev başlatma ve durumunu ortak biçimde raporlama.
- Kaynak durumları ve altyapı hatalarını ortak modele dönüştürme.
- Gerektiği ölçüde depolama ve ağ işlemleri.

İlk günden genel amaçlı çoklu motor çerçevesi kurmayın; yalnızca gerçek ihtiyaçları soyutlayın.

## Proxmox'a özgü kalacak ayrıntılar
Düğüm/küme kavramları, Proxmox görev kimlikleri ve API hata biçimleri, depolama türleri ve API kimlik doğrulama ayrıntıları adaptör içinde tutulur. Ürün API'sine sızmaları gerekiyorsa ortak modele çevrilir.

## Güvenlik gereksinimleri
- Kiracı izolasyonu yalnızca arayüzde değil, sunucu tarafında uygulanır.
- Kullanıcı izinleri ve kaynak kapsamı her istekte kontrol edilir.
- Web uygulamasına sınırsız root/administrator yetkisi verilmez.
- Gizli anahtarlar kaynak kodda tutulmaz ve loglara yazılmaz.
- Kritik işlemlerde aktör, zaman, kaynak, işlem ve sonuç kaydedilir.
- Silme, disk değiştirme ve konsol erişimi gibi işlemler için ek kontroller değerlendirilir.

## İlk sürümde vaat edilmeyenler
Yüksek erişilebilirlik, canlı taşıma, çok düğümlü küme yönetimi, dağıtık depolama, gelişmiş SDN, faturalandırma ve Kubernetes entegrasyonu.

## Alternatif altyapı değerlendirmesi
KVM/QEMU/libvirt tabanlı alternatif ancak lisans, işletim maliyeti, özelleştirme ihtiyacı veya teknik gereksinimler gerekçe oluşturursa prototiplenir. Karar takvime değil ölçülebilir ihtiyaçlara dayanır.

## Karar günlüğü
| Tarih | Karar | Gerekçe |
|---|---|---|
| 2026-10-19 | İlk sürüm Proxmox VE API'si ile başlayacak | Tek geliştirici için uygulanabilir başlangıç |
| 2026-10-19 | Ürün API'si ile sanallaştırma adaptörü ayrılacak | Gelecekte alternatif altyapı değerlendirmesi |
| 2026-10-19 | İlk hedef tek sunucu | MVP kapsamını sınırlamak |
| 2026-10-19 | Proje lisansı AGPL-3.0-only olarak belirlendi | Ağ üzerinden hizmet sunulan değiştirilmiş sürümler için de lisansın kaynak sunma koşullarını korumak |
