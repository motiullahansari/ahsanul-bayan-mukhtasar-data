# Ahsanul Bayan - Mukhtasar (Hindi) — Data

UmmahTech ke **Ahsanul Bayan - Mukhtasar** app ka data (Hindi translation + mukhtasar tafseer).
App pehli baar khulne par ye files download karke phone me save kar leta hai.

## Files (`v1/`)
| File | Kya hai |
|---|---|
| `manifest.json` | Version, har file ka size aur SHA-256 (app isse check karta hai) |
| `surahs.json` | 114 surahon ki list: `n, name, meaning, place, ayat_count, juz, page` |
| `surah/001.json … 114.json` | Har surah ki ayaten: `n, juz, page, translation, text, notes[]` |

- `translation` — saaf translation, bina footnote number
- `text` — `[1]` `[2]` markers ke saath
- `notes` — tafseer: `[{ "n": 1, "text": "…" }]`, `n` ayat ke `[n]` se juda

## URLs
- CDN: `https://cdn.jsdelivr.net/gh/motiullahansari/ahsanul-bayan-mukhtasar-data@main/v1/<file>`
- Raw: `https://raw.githubusercontent.com/motiullahansari/ahsanul-bayan-mukhtasar-data/main/v1/<file>`

## Data update kaise karein
1. `v1/` me files badlo
2. `manifest.json` me `version` +1 karo (aur sha256/bytes dobara banao)
3. Push karo — app agli baar naya version dekh kar data dobara download karega
