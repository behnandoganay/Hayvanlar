# Ses kaynakları

Bu klasördeki sesler hazır kayıtlardan hazırlandı. Dosya adları indirildikleri
sırada Pixabay katkıcı adlarını taşıyordu; izlenebilir olsun diye buraya yazıldı.

| Dosya         | Özgün dosya adı                                   | Katkıcı             |
|---------------|---------------------------------------------------|---------------------|
| `inek.mp3`    | `dragonstudio-cow-moo-1-472361.mp3`               | dragonstudio        |
| `koyun.mp3`   | `universfield-sheep-bleat-122256.mp3`             | universfield        |
| `keci.mp3`    | `dragonstudio-goat-baa-390303.mp3`                | dragonstudio        |
| `kopek.mp3`   | `dragonstudio-free-dog-bark-419014.mp3`           | dragonstudio        |
| `kedi.mp3`    | `dragonstudio-cat-meow-401729.mp3`                | dragonstudio        |
| `ordek.mp3`   | `freesound_community-075176-duck-quack-40345.mp3` | freesound_community |
| `kurbaga.mp3` | `dragonstudio-frog-croaking-sound-effect-322956.mp3` | dragonstudio     |
| `at.mp3`      | `dragonstudio-horse-neigh-390297.mp3`             | dragonstudio        |

### İneğin ilk kaydı neden değişti

İlk denenen inek kaydı (`u_jd81cxyq22-cow-mooing-343423.mp3`) kulağa kötü geliyordu.
Ölçüldüğünde teknik bir bozulma bulunamadı — kırpma yoktu, kanalları zaten aynıydı,
mp3'e kodlama da zarar vermemişti. Sorun kaydın kendisindeydi, o yüzden değiştirildi.

## Lisans

Dosya adları Pixabay kaynaklı olduklarını gösteriyor. Pixabay'in içerik lisansı
kaynak belirtmeyi zorunlu tutmaz; bu tablo yine de nereden geldiklerini kaydetmek için var.

> Bu dosyaları hazırlarken internet erişimim yoktu, lisans koşullarını kendim
> doğrulayamadım. Uygulamayı herkese açık yayınlayacaksanız indirdiğiniz
> sayfalardaki koşulları bir kez gözden geçirin.

## Yapılan işlemler

Kayıtlar olduğu gibi kullanılmadı; hepsi aynı işlemden geçirildi:

- **Baştaki sessizlik kırpıldı** (20 ms pay bırakılarak). En kötüsü inekti: 0.37 saniye.
  Bu kadar gecikme çocuğa "dokundum ama bir şey olmadı" hissi veriyor.
- **Sondaki sessizlik kırpıldı.** Ördekte 2.65 saniye boş kuyruk vardı.
- **Kurbağa kısaltıldı** — 8.1 saniyelik kayıttan 0.05–1.90 saniye arası alındı;
  bu pencere tam üç vıraklama içeriyor.
- **Seviyeler eşitlendi.** Kaynaklar arasında 7.5 kat (yaklaşık 17 dB) gürlük farkı
  vardı: kedi bağırırken kurbağa duyulmuyordu. Hepsi aynı RMS'e getirildi,
  tepe değerler 0.95 ile sınırlandı (ineğin kaynağı zaten kırpılmıştı).
- **8 ms açılış / 40 ms kapanış yumuşatması** — kesme yerlerinde "tık" olmasın diye.
- **İnekte kanal seçimi ve kırpma onarımı yapıldı.** Bu kaydın sol ve sağ kanalları
  birbirinden hayli farklıydı (uyum 0.24); düpedüz mono'ya toplamak 2.09 dB enerji
  kaybettiriyor, yani kanallar birbirini kısmen iptal edip sesi içi boş yapıyordu.
  Sağ kanal ayrıca ciddi kırpılmıştı (562 örnek, art arda 15'e kadar). Bu yüzden
  daha temiz olan sol kanal alındı ve kalan 9 kırpma dizisi (45 örnek) kübik ara
  değerlemeyle onarıldı.
- **Mono, 48 kHz, 128 kbps'e dönüştürüldü.** Kaynaklar stereo 256 kbps'ti;
  bu uygulama için gereksiz. Toplam 632 KB'den 151 KB'ye indi.
