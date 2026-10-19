# Katkıda Bulunma Rehberi

Projeye katkılar memnuniyetle değerlendirilir. Kabul edilen değişikliklerin kapsamı ve ana dala birleştirilmesi proje sahibinin incelemesine tabidir.

## Katkı akışı
1. Mevcut Issue'ları ve belgeleri inceleyin.
2. Büyük değişikliklerden önce Issue açıp yaklaşımı tartışın.
3. Depoyu fork edin ve kendi fork'unuzda ayrı bir dalda çalışın.
4. Testleri çalıştırın; gerekli belgeleri güncelleyin.
5. Ana depoya Pull Request (PR) açın.
6. İnceleme geri bildirimlerine göre değişiklik yapın.

Dış katkıcıların başlangıçta ana depoya doğrudan yazma yetkisi yoktur. Güvenilir katkıcılara ileride ihtiyaç ve güven düzeyine göre sınırlı yazma yetkisi verilebilir. Bu durum, `main` dalının koruma ve inceleme kurallarını otomatik olarak kaldırmaz.

## Pull Request kontrol listesi
- [ ] Amaç ve gerekçe açıklandı.
- [ ] İlgili Issue bağlandı (varsa).
- [ ] Testler eklendi veya çalıştırıldı; çalıştırılamadıysa sebebi açıklandı.
- [ ] Güvenlik ve kiracı/yetki sınırı etkileri değerlendirildi.
- [ ] Terminoloji `GLOSSARY.md` ile tutarlı.
- [ ] Belgeler güncellendi.
- [ ] Gizli anahtar, parola, token, kişisel veri veya üretim verisi eklenmedi.
- [ ] Yeni bağımlılıkların lisansları ve bakım durumu kontrol edildi.

## Kod ve mimari ilkeleri
- Değişiklikleri mümkün olduğunca küçük ve tek amaçlı tutun.
- Arayüzdeki kontrolleri sunucu tarafı yetkilendirmenin yerine koymayın.
- Web uygulamasından sınırsız root/administrator komutu çalıştırmayın.
- Proxmox'a özgü kodu sanallaştırma adaptörü sınırında tutun.
- Yeni bağımlılıkların gerekçesini ve lisansını PR açıklamasında belirtin.
- Güvenlik açığı ayrıntılarını herkese açık Issue/PR olarak yayımlamayın; `SECURITY.md` dosyasını izleyin.

## Terminoloji
`GLOSSARY.md` projenin terminoloji kaynağıdır. Yeni terim eklemeden önce mevcut terimleri kontrol edin. Aynı kavram için yeni eş anlamlı üretmeyin. Terim kimliklerini değiştirmeyin. Sözlük değişikliklerini gerekçesiyle açıklayın.

## Lisans ve katkı hakları
Proje **GNU Affero Genel Kamu Lisansı v3.0-only (`AGPL-3.0-only`)** altında yayımlanır; tam metin `LICENSE` dosyasındadır. Pull Request göndermek, katkının bu proje lisansı altında yayımlanmasını kabul ettiğiniz anlamına gelir. Katkı üzerinde gerekli haklara sahip olduğunuzdan ve katkıyı bu lisans koşullarıyla sunmaya yetkili olduğunuzdan emin olun. Şu aşamada ayrı bir CLA veya telif devri şartı uygulanmaz.

Üçüncü taraf kod, metin, ikon veya başka materyal ekliyorsanız kaynağını ve lisansını PR'da belirtin; lisansı belirsiz veya uyumsuz olabilecek materyali eklemeyin. Projenin AGPL-3.0-only lisansı, bağımlılıkların ya da Proxmox VE'nin kendi lisans koşullarını ortadan kaldırmaz. Gerekirse lisans uyumluluğunu PR birleştirilmeden önce ayrıca değerlendirin.

## İnceleme ve karar
PR; teknik kalite, güvenlik, kapsam, bakım maliyeti, terminoloji, lisans ve proje hedeflerine uygunluk açısından incelenir. PR kabul edilebilir, değişiklik istenebilir, ertelenebilir veya gerekçesiyle kapatılabilir.
