# Lisans ve Üçüncü Taraf Bileşen Politikası

## Proje lisansı

**Karar:** Bu projenin kendi kodu GNU Affero Genel Kamu Lisansı v3.0-only (`AGPL-3.0-only`) altında yayımlanır. Resmî lisans metni depodaki [`LICENSE`](LICENSE) dosyasındadır.

SPDX lisans tanımlayıcısı: `AGPL-3.0-only`  
Resmî lisans bilgisi: <https://www.gnu.org/licenses/agpl-3.0.html>  
SPDX kaydı: <https://spdx.org/licenses/AGPL-3.0-only.html>

Bu karar, "AGPL-3.0-or-later" anlamına gelmez; yalnızca AGPL sürüm 3 seçilmiştir. Bu belge lisans metninin yerine geçmez.

## Proxmox VE ile çalışma

Proxmox VE ile entegrasyonun ilk aşamada Proxmox VE API'si üzerinden yapılması planlanır. Proxmox VE'nin kendi kodu, paketleri, markaları ve diğer bileşenleri kendi lisans ve kullanım koşullarına tabi olmaya devam eder. Projenin `AGPL-3.0-only` lisansı, Proxmox VE'ye ait bileşenlerin lisansını değiştirmez veya bunların kullanımına tek başına izin vermez.

- Proxmox VE'den kod kopyalamadan önce ilgili dosya ve bileşenin lisansını kontrol edin.
- Her yeni bağımlılığın lisansını, sürümünü ve kaynağını kaydedin.
- Bir bağımlılığın AGPL-3.0-only ile uyumluluğu belirsizse eklemeden önce inceleme isteyin.
- Proxmox adı ve logosunu kullanırken ilgili marka ve görsel kullanım koşullarını ayrıca değerlendirin.
- Mimari sınırları koruyun: Proxmox'a özgü entegrasyonu mümkün olduğunca sanallaştırma adaptöründe tutun. Bu tasarım tek başına hukuki uyumluluk garantisi değildir.

## Katkılar

Katkılar kabul edildiğinde proje lisansı altında yayımlanır. Katkıcılar katkı üzerinde gerekli haklara sahip olduklarından ve üçüncü taraf materyalleri kullanma yetkileri bulunduğundan emin olmalıdır. Şu aşamada ayrı bir Contributor License Agreement (CLA) veya telif devri şartı uygulanmaz.

## Lisans uyumluluğu kontrol listesi

Yeni bir bağımlılık veya üçüncü taraf materyal eklerken:

1. Kaynak URL'sini, adı ve sürümünü kaydedin.
2. Lisans tanımlayıcısını ve lisans metnini doğrulayın.
3. Lisansın kullanım, değiştirme, dağıtım ve ağ üzerinden sunum koşullarını değerlendirin.
4. Gerekli telif, lisans ve NOTICE bildirimlerini koruyun.
5. Sonucu PR açıklamasında belirtin; belirsiz durumda birleştirmeden önce inceleme talep edin.

Bu belge genel proje politikasıdır; hukuki danışmanlık değildir. Karmaşık entegrasyon veya dağıtım senaryolarında uzman hukuki değerlendirme gerekebilir.
