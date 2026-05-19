# Ma'muriy bo'linish ma'lumotlari

O'zbekistonning to'liq ma'muriy bo'linish ma'lumotlari — viloyat, tuman/shahar va mahalla darajasida.

## Fayllar

### Lotin yozuvida (kenjebaev/regions manbasi — ID'lar mos)

| Fayl | Soni | Tavsifi |
|---|---|---|
| `regions-latin.json` | 14 | Viloyatlar va Qoraqalpog'iston Respublikasi |
| `districts-latin.json` | 203 | Tumanlar va shaharlar (`region_id` orqali viloyatga bog'lanadi) |
| `mahallas-latin.json` | 10,035 | Mahallalar/MFY (`district_id` orqali tumanga bog'lanadi) |

### Kirill yozuvida (MIMAXUZ manbasi — alohida ID'lar)

| Fayl | Soni | Tavsifi |
|---|---|---|
| `regions-cyrillic.json` | 14 | `name_oz` maydonida Kirill nomlar, `name_uz` Lotin, `name_ru` Rus |
| `districts-cyrillic.json` | 210 | Yana 3 tilda nomlar |

## Ma'lumot tuzilmasi

**Lotin versiyada** (kenjebaev):
```json
// regions-latin.json
{ "id": 2, "name": "Andijon viloyati" }

// districts-latin.json
{ "id": 16, "region_id": 2, "name": "Oltinko'l tumani" }

// mahallas-latin.json
{ "id": 1, "district_id": 15, "name": "Amir Temur nomli ovul fuqarolar yig'ini" }
```

**Kirill versiyada** (MIMAXUZ):
```json
{
  "id": 2,
  "soato_id": 1703,
  "name_uz": "Andijon viloyati",
  "name_oz": "Андижон вилояти",
  "name_ru": "Андижанская область"
}
```

## Manbalar

- [kenjebaev/regions](https://github.com/kenjebaev/regions) — Lotin, to'liq iyerarxiya
- [MIMAXUZ/uzbekistan-regions-data](https://github.com/MIMAXUZ/uzbekistan-regions-data) — Kirill+Lotin+Rus
