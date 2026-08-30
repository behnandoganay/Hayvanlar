# Gerçek hayvan sesleri (isteğe bağlı)

Uygulama sesleri kendi üretiyor, yani **bu klasör boş olsa da her şey çalışır**.

Ama gerçek hayvan kayıtları kullanmak isterseniz, mp3 dosyalarını tam olarak
şu adlarla bu klasöre koymanız yeterli:

| Hayvan  | Dosya adı      |
|---------|----------------|
| İnek    | `inek.mp3`     |
| Koyun   | `koyun.mp3`    |
| Keçi    | `keci.mp3`     |
| Köpek   | `kopek.mp3`    |
| Kedi    | `kedi.mp3`     |
| Ördek   | `ordek.mp3`    |
| Kurbağa | `kurbaga.mp3`  |
| At      | `at.mp3`       |

Dosya adlarında Türkçe harf **yok** (ö, ç, ğ yerine o, c, g) — bazı sunucular
Türkçe karakterli dosya adlarında sorun çıkarıyor.

Uygulama açılırken her dosyayı tek tek yokluyor:

- Dosya varsa → o hayvana dokunulduğunda **gerçek kayıt** çalar.
- Dosya yoksa → sessizce **üretilen ses** çalmaya devam eder.

Yani hepsini birden koymak zorunda değilsiniz; sadece `inek.mp3` koyarsanız
yalnız inek gerçek sesle, diğerleri üretilen sesle çalar.

## Nelere dikkat etmeli

- **Kısa tutun** — 1–2 saniye ideal. Uzun kayıtlarda çocuk bir sonrakine
  geçmek için beklemek zorunda kalıyor.
- **Sesleri birbirine yakın seviyede** kaydedin, biri diğerinden çok yüksek olmasın.
- **Telif** — internetten bulduğunuz her sesi kullanamazsınız. Ücretsiz ve serbest
  kaynaklar için "CC0" veya "public domain" etiketli ses arşivlerine bakın.
