# Proje Sözlüğü

Bu dosya, arayüz, API, kod ve dokümantasyondaki terimler için ortak referanstır. Terim değişiklikleri `CONTRIBUTING.md` kurallarına tabidir.

## Yönetim kuralları
1. Yeni terim eklemeden önce mevcut terimleri ve eş anlamlıları kontrol edin.
2. Terim kimlikleri kalıcıdır; silinmez ve başka kavrama atanmaz.
3. Onaylı terim tanımları gerekçesiz değiştirilmez.
4. Karara bağlanmamış terimler Taslak olarak işaretlenir.
5. Kullanımdan kaldırılan terim silinmez; yerine geçen terim belirtilir.
6. Türkçe arayüz adı ile kod/API teknik adı ayrı kaydedilebilir.
7. Teknik standartları ve komutları zorla Türkçeleştirmeyin.

## Terimler

### TERM-0001 — Sanal makine
- **İngilizce/teknik karşılık:** Virtual Machine (VM)
- **Tanım:** Sanal donanım üzerinde çalışan, kendi işletim sistemine ve uygulamalarına sahip mantıksal bilgisayar.
- **Kullanım:** İlk kullanımda “Sanal makine (VM)”; sonra “sanal makine” veya bağlam uygunsa “VM”.
- **Durum:** Onaylı

### TERM-0002 — Ana makine
- **İngilizce/teknik karşılık:** Host / Hypervisor host
- **Tanım:** Sanal makineleri çalıştıran fiziksel sunucu.
- **Durum:** Onaylı

### TERM-0003 — Sanallaştırma altyapısı
- **İngilizce/teknik karşılık:** Virtualization infrastructure
- **Tanım:** Sanal makineleri çalıştıran hipervizör, işlemci/bellek kaynakları, depolama, sanal ağ ve yönetim bileşenlerinin bütünü.
- **Durum:** Onaylı

### TERM-0004 — Hipervizör
- **İngilizce/teknik karşılık:** Hypervisor
- **Tanım:** Sanal makinelerin donanım kaynaklarını kullanmasını ve birbirinden yalıtılmasını sağlayan sanallaştırma katmanı.
- **Kullanım:** Proxmox VE yalnızca hipervizör olarak adlandırılmaz; daha kapsamlı bir yönetim platformudur.
- **Durum:** Onaylı

### TERM-0005 — Sanal işlemci
- **İngilizce/teknik karşılık:** Virtual CPU (vCPU)
- **Tanım:** Sanal makineye sunulan sanal işlemci kapasitesi.
- **Kullanım:** vCPU sayısı fiziksel çekirdek sayısıyla bire bir eşdeğer gibi sunulmamalıdır.
- **Durum:** Onaylı

### TERM-0006 — Bellek
- **İngilizce/teknik karşılık:** Memory / RAM
- **Tanım:** Sanal makineye tahsis edilen veya ana makinede bulunan çalışma belleği.
- **Durum:** Onaylı

### TERM-0007 — Depolama
- **İngilizce/teknik karşılık:** Storage
- **Tanım:** Sanal disk, imaj, yedek veya kalıcı verilerin tutulduğu kaynak/hizmet.
- **Durum:** Onaylı

### TERM-0008 — Sanal disk
- **İngilizce/teknik karşılık:** Virtual disk
- **Tanım:** Sanal makineye disk aygıtı olarak sunulan mantıksal disk.
- **Kullanım:** Sanal kapasite ile fiilen kullanılan fiziksel alan aynı olmayabilir.
- **Durum:** Onaylı

### TERM-0009 — Sanal ağ
- **İngilizce/teknik karşılık:** Virtual network
- **Tanım:** Sanal makineler ve/veya fiziksel ağlar arasında sanal bağlantı sağlayan ağ yapılandırması.
- **Durum:** Onaylı

### TERM-0010 — Ağ köprüsü
- **İngilizce/teknik karşılık:** Network bridge
- **Tanım:** Ağ trafiğini katman 2 düzeyinde arayüzler arasında iletebilen sanal ağ bileşeni.
- **Kullanım:** `vmbr0` gibi altyapı adları teknik ayrıntılarda özgün bırakılabilir.
- **Durum:** Onaylı

### TERM-0011 — Kiracı
- **İngilizce/teknik karşılık:** Tenant
- **Tanım:** Platformda kendisine ait kullanıcıları, izinleri ve kapsamı olan mantıksal müşteri/organizasyon alanı.
- **Kullanım:** Gerekirse ilk kullanımda “Kiracı (organizasyon alanı)” açıklaması gösterilir.
- **Durum:** Onaylı

### TERM-0012 — Rol
- **İngilizce/teknik karşılık:** Role
- **Tanım:** Kullanıcının hangi işlemleri yapabileceğini belirleyen izin kümesi.
- **Durum:** Onaylı

### TERM-0013 — Yetki kapsamı
- **İngilizce/teknik karşılık:** Permission scope
- **Tanım:** İzinlerin hangi kiracı veya kaynaklar üzerinde geçerli olduğunu belirleyen sınır.
- **Durum:** Onaylı

### TERM-0014 — Görev
- **İngilizce/teknik karşılık:** Task / Job
- **Tanım:** Başlatılan ve sonucu takip edilen işlem; örneğin sanal makine oluşturma veya başlatma.
- **Durum:** Onaylı

### TERM-0015 — Denetim kaydı
- **İngilizce/teknik karşılık:** Audit log
- **Tanım:** Kim tarafından, ne zaman, hangi kaynakta hangi işlemin yapıldığını ve sonucunu kaydeden kayıt.
- **Durum:** Onaylı

### TERM-0016 — Sanallaştırma adaptörü
- **İngilizce/teknik karşılık:** Virtualization adapter
- **Tanım:** Ürünün ortak arayüzünü belirli sanallaştırma altyapısının API veya mekanizmalarına bağlayan bileşen.
- **Kullanım:** İlk adaptör Proxmox VE için olacaktır.
- **Durum:** Onaylı

### TERM-0017 — Sanallaştırma yönetim platformu
- **İngilizce/teknik karşılık:** Virtualization management platform
- **Tanım:** Sanal makineleri, kaynakları, kullanıcıları, izinleri ve görevleri yöneten ürünün bütünü.
- **Durum:** Onaylı

### TERM-0018 — Kaynak
- **İngilizce/teknik karşılık:** Resource
- **Tanım:** Platformun görüntülediği veya yönettiği varlık ya da kapasite; örneğin VM, ağ, depolama veya işlemci/bellek.
- **Kullanım:** Belirsizse kaynak türünü belirtin.
- **Durum:** Onaylı

### TERM-0019 — Küme
- **İngilizce/teknik karşılık:** Cluster
- **Tanım:** Birden fazla ana makinenin ortak yönetim veya çalışma amacıyla ilişkilendirildiği altyapı yapısı.
- **Kullanım:** Tek sunuculu ilk sürüm küme yönetimi destekliyormuş gibi tanıtılmamalıdır.
- **Durum:** Onaylı

### TERM-0020 — Yüksek erişilebilirlik
- **İngilizce/teknik karşılık:** High Availability (HA)
- **Tanım:** Belirli arızalarda hizmetin tanımlanmış kesinti hedefleri içinde devam etmesini veya yeniden sunulmasını sağlayan tasarım.
- **Kullanım:** Tek sunuculu sürüm, doğrulanmış ek mekanizma olmadan yüksek erişilebilir olarak adlandırılmamalıdır.
- **Durum:** Onaylı

## Taslak terimler
| Terim | Öneri | Açıklama | Durum |
|---|---|---|---|
| Snapshot | Anlık görüntü | Yedeklemeden farkı tanımlanmalı | Taslak |
| Template | Şablon | VM şablonu ile ayar şablonu ayrılmalı | Taslak |
| Image | İmaj | ISO, disk ve makine imajı ayrımı yapılmalı | Taslak |
| Quota | Kaynak kotası | Aşım davranışı tanımlanmalı | Taslak |
| Console | Konsol | Erişim ve yetki sınırı tanımlanmalı | Taslak |
| Backup / Restore | Yedekleme / Geri yükleme | Felaket kurtarmadan ayrıştırılmalı | Taslak |

## Yeni terim şablonu
```markdown
### TERM-XXXX — Tercih edilen Türkçe terim
- **İngilizce / teknik karşılık:**
- **Tanım:**
- **Kullanım notu:**
- **Tercih edilmeyen ifadeler:**
- **Durum:** Taslak
- **İlgili terimler:**
```

## Değişiklik günlüğü
| Tarih | Değişiklik | Gerekçe |
|---|---|---|
| 2026-10-19 | İlk sürüm oluşturuldu | Ortak terminoloji referansı |
