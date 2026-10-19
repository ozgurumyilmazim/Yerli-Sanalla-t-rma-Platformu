# Yerli Sanallaştırma Platformu

> **Durum:** Erken planlama ve geliştirme aşaması. Üretim ortamında kullanıma hazır olduğu iddia edilmez.

Kurumsal şirketler ve veri merkezleri için Türkçe kullanım deneyimine öncelik veren açık kaynaklı sanallaştırma yönetim platformu geliştirme girişimi.

## Amaç
- Sanal makineleri ve temel altyapı kaynaklarını anlaşılır bir Türkçe arayüzden yönetmek.
- İleri düzey kullanıcılar için teknik ayrıntıları ve özgün komutları korumak.
- Çok kiracılı kullanıcı ve yetkilendirme modelini güvenli tasarlamak.
- İlk aşamada Proxmox VE API'si üzerinden çalışmak.
- Ürün kodunu bir sanallaştırma adaptörü arkasında tutarak ileride KVM/QEMU/libvirt seçeneklerini değerlendirmek.

## İlk sürüm kapsamı
İlk prototip tek sunucuya odaklanır. Öncelikler: sanal makine listeleme ve temel yaşam döngüsü, kaynak görünümü, kullanıcı/rol yönetimi, görev takibi ve denetim kayıtları.

İlk sürüm için küme yönetimi, yüksek erişilebilirlik, canlı taşıma, dağıtık depolama, gelişmiş SDN, faturalandırma veya Kubernetes entegrasyonu vaat edilmez.

## Belgeler
- [Mimari](ARCHITECTURE.md)
- [Proje sözlüğü](GLOSSARY.md)
- [Katkıda bulunma rehberi](CONTRIBUTING.md)
- [Davranış kuralları](CODE_OF_CONDUCT.md)
- [Güvenlik politikası](SECURITY.md)
- [Lisans ve üçüncü taraf bileşen politikası](LICENSE-POLICY.md)

## Katkıda bulunma
Katkılar Issue ve Pull Request üzerinden önerilir. Ana dala birleştirme kararı proje sahibine aittir. Başlamak için `CONTRIBUTING.md` dosyasını okuyun.

## Lisans
Bu proje **GNU Affero Genel Kamu Lisansı v3.0-only (`AGPL-3.0-only`)** altında yayımlanır. Lisansın tam metni [`LICENSE`](LICENSE) dosyasındadır. Lisansın ağ üzerinden etkileşim ve kaynak kodu sunma koşulları dâhil olmak üzere tüm hükümleri geçerlidir.

Proxmox VE ve diğer üçüncü taraf bileşenler kendi lisanslarına tabi olabilir. Bu projenin lisansı, üçüncü taraf yazılımların lisansını değiştirmez; ayrıntılar için [`LICENSE-POLICY.md`](LICENSE-POLICY.md) dosyasına bakın.
