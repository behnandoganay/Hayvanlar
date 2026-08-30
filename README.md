# Hayvanlar

Küçük çocuklar için sesli hayvan uygulaması. Ekranda sevimli hayvan resimleri var;
birine dokununca o hayvanın sesi çıkıyor ve resim zıplıyor.

İlk sürümdeki hayvanlar: **inek, koyun, keçi, köpek, kedi, ördek, kurbağa, at**.

## Nasıl açılır

`index.html` dosyasına çift tıklayın. Hepsi bu.

- Kurulum yok, internet gerekmez, hiçbir şeye üye olmanız gerekmez.
- Bilgisayar, tablet, telefon — hepsinde tarayıcıda çalışır.
- Telefonda 2 sütun, tablette 4 sütun olarak kendini ayarlar.

### Tablette ana ekrana eklemek

Uygulama gibi tam ekran açılması için:

- **iPad / iPhone (Safari):** Paylaş ➝ *Ana Ekrana Ekle*
- **Android (Chrome):** ⋮ menüsü ➝ *Ana ekrana ekle*

### İnternette yayınlamak (isteğe bağlı)

GitHub'da: **Settings → Pages → Source: Deploy from a branch** ve bu dalı seçin.
Birkaç dakika sonra çocuğunuza verebileceğiniz bir adres oluşur.

## Sesler

Sesler tarayıcıda **Web Audio** ile anlık olarak üretiliyor — depoda hiç ses dosyası yok.
Bu yüzden uygulama internetsiz de, hiçbir şey indirmeden de çalışıyor.

Sesler çizgi film tarzıdır, gerçek hayvan kaydı değildir. Gerçek kayıt kullanmak
isterseniz `sesler/` klasörüne mp3 koymanız yeterli — uygulama otomatik onları çalar.
Ayrıntılar: [`sesler/README.md`](sesler/README.md)

> Tarayıcı geliştirici konsolunda `sesler/*.mp3` için 404 uyarıları görürseniz bu normaldir:
> uygulama gerçek kayıt var mı diye yokluyor, yoksa kendi ürettiği sesle devam ediyor.

## Çocuk için düşünülmüş ayrıntılar

- Aynı anda tek ses çalar — çocuk butonlara arka arkaya bastığında sesler üst üste binmez.
- Her çalışta ses hafifçe farklı perdeden çıkar, tekrar tekrar basınca robotik durmaz.
- Çift dokunuşta sayfa yakınlaşmaz, uzun basınca metin seçimi/menü açılmaz.
- Aşağı çekince sayfa yenilenmez.
- Dokunma hedefleri büyüktür; ses `pointerdown` ile çalar, yani parmak değer değmez.
- Cihazda "hareketi azalt" ayarı açıksa animasyonlar kendiliğinden kapanır.

## Yeni hayvan eklemek

Üç şey gerekiyor:

1. `index.html` içine, diğerlerinin yanına `data-hayvan="tavuk"` şeklinde bir
   `<button class="kart">` ve içine SVG çizimi.
2. Aynı dosyadaki `SENTEZ` nesnesine `tavuk: function (ctx, hedef, t0) { ... }`
   biçiminde bir ses reçetesi (var olanları örnek alabilirsiniz).
3. Ya da sentezle uğraşmadan `sesler/tavuk.mp3` koyun — o zaman 2. adım gerekmez.

## Dosyalar

| Dosya            | Ne işe yarar                                     |
|------------------|--------------------------------------------------|
| `index.html`     | Uygulamanın tamamı — HTML, CSS, JavaScript, çizimler |
| `sesler/`        | İsteğe bağlı gerçek hayvan sesi mp3'leri         |
