# Vardiya Planlayıcı

3 vardiya (Sabah/Öğlen/Gece) otomatik personel planlama aracı.

## Özellikler
- **Otomatik üret**: 6/6/3 kadroyu, dinlenme (11s) ve ardışık gün (max 6) kurallarına uyarak dağıtır
- **Canlı kural denetimi**: her düzenlemede dinlenme/ardışık/haftalık/kadro ihlallerini gösterir
- **Net saat + maliyet**: 8s brüt − 0,5s mola = 7,5s net; saat ücretiyle aylık işçilik
- **Kişi kısıtları**: "gece yapamaz" işareti, kişiye özel ücret
- Aylar arası geçiş, Excel export, yazdırma, otomatik kayıt (tarayıcı)

## Deploy (Cloudflare Pages)
Tek dosya, build gerekmez.

```bash
# Cloudflare'e deploy
export CLOUDFLARE_API_TOKEN="<cf_token>"
export CLOUDFLARE_ACCOUNT_ID="ac6ab4ce1149a3591d014841856490af"
npx wrangler pages deploy . --project-name=vardiya-planlayici
```

Canlı adres: https://vardiya-planlayici.pages.dev
