# Güvenlik Politikası

## Desteklenen sürümler
Proje erken geliştirme aşamasındadır; kararlı sürüm veya resmi güvenlik destek takvimi henüz yoktur.

## Güvenlik açığı bildirme
İstismar edilebilir açıkların ayrıntılarını herkese açık Issue veya Pull Request olarak yayımlamayın. GitHub deposu oluşturulduğunda, GitHub'ın **Private vulnerability reporting** özelliği mevcutsa etkinleştirin ve bu bölümü gerçek bildirim yoluna göre güncelleyin. Özel kanal etkin değilse, istismar ayrıntılarını paylaşmadan önce proje sahibinden özel iletişim kanalı isteyin.

Bildirime etkilenen sürüm/commit, etki, güvenli yeniden üretim adımları ve varsa azaltma önerisi eklenebilir. Gerçek parola, token, müşteri verisi veya hassas üretim günlüğü eklemeyin.

## Temel güvenlik ilkeleri
- Her istekte sunucu tarafı yetkilendirme ve kiracı kapsamı kontrolü.
- En az ayrıcalık; web uygulamasından sınırsız root komutu çalıştırmama.
- Gizli bilgileri kaynak kodda veya loglarda tutmama.
- Kritik işlemler için denetim kaydı.
- Girdi doğrulama ve güvenli hata yönetimi.
- Bağımlılıkları, yedekleme/geri yükleme ve güncelleme süreçlerini düzenli test etme.
