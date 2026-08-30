# Gerçek hayvan seslerini buraya koyun

Dosyaları **tam olarak bu adlarla** bu klasöre (`sesler/`) koymanız yeterli.
Başka hiçbir şey yapmanıza gerek yok — uygulama açılışta bakıyor ve buluyor.

| Hayvan  | Dosya adı     | Aranacak İngilizce terim |
|---------|---------------|--------------------------|
| İnek    | `inek.mp3`    | cow moo                  |
| Koyun   | `koyun.mp3`   | sheep baa / sheep bleat  |
| Keçi    | `keci.mp3`    | goat bleat               |
| Köpek   | `kopek.mp3`   | dog bark                 |
| Kedi    | `kedi.mp3`    | cat meow                 |
| Ördek   | `ordek.mp3`   | duck quack               |
| Kurbağa | `kurbaga.mp3` | frog croak               |
| At      | `at.mp3`      | horse neigh              |

**Dosya adlarında Türkçe harf yok** — `ö, ç, ğ, ı` yerine `o, c, g, i` yazın.
Bazı sunucular Türkçe karakterli adlarda sorun çıkarıyor.

**Hepsini birden koymak zorunda değilsiniz.** Sadece `inek.mp3` koyarsanız
yalnızca inek gerçek sesle çalar, kalanlar üretilen sesle devam eder.

**mp3 şart değil.** `m4a`, `ogg` ve `wav` de çalışır — indirdiğiniz dosya
hangi biçimdeyse uzantısını değiştirmeden koyun (`inek.wav` gibi).
Uygulama sırayla mp3 → m4a → ogg → wav diye bakıyor.

## Nereden bulunur

> Bu adresleri size önerirken internete bakamadım, o yüzden indirmeden önce
> sayfadaki lisans bilgisini kendiniz görün.

- **Pixabay** — `pixabay.com/sound-effects/` — üyelik istemez, doğrudan mp3
  indirtir, kaynak belirtme zorunluluğu yoktur. Başlamak için en kolayı.
- **Freesound** — `freesound.org` — çok geniş arşiv, ücretsiz üyelik ister.
  Filtrelerden **CC0** seçerseniz hiçbir koşulu olmayan sesleri görürsünüz.
- **Wikimedia Commons** — `commons.wikimedia.org` — kamuya açık kayıtlar;
  çoğu `ogg` veya `wav` biçiminde, ikisi de doğrudan çalışıyor.
- **BBC Sound Effects** — `sound-effects.bbcrewind.co.uk` — kişisel kullanım
  için ücretsiz, `wav` indirir.

## Seçerken nelere dikkat edin

- **Kısa olsun** — 1–2 saniye ideal. Uzun kayıtta çocuk bir sonraki hayvana
  geçmek için beklemek zorunda kalıyor.
- **Baştaki sessizliği kırpın.** En sık yapılan hata bu: dosyanın başında
  yarım saniye sessizlik varsa çocuk dokunuyor, hemen ses gelmiyor ve
  uygulama bozuk sanılıyor. Ses dosyanın ilk anında başlamalı.
- **Ses seviyeleri birbirine yakın olsun**, biri diğerinden çok gür olmasın.
- **Tek hayvan olsun** — arka planda çiftlik gürültüsü, müzik veya insan
  sesi olan kayıtları seçmeyin.
