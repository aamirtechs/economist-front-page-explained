# The JSON API

[Back to the full index](README.md)

Everything on this site is also available as free JSON data, served from the same GitHub Pages site. No key, no signup, no cost. The files are updated whenever the project is updated.

**Base URL:** `https://aamirtechs.github.io/economist-front-page-explained/api/`

## Endpoints

| Endpoint | What it returns |
|---|---|
| [covers.json](api/covers.json) | All 62 covers: year, date, cover name, theme, the prediction, its status, and what actually happened |
| [summary.json](api/summary.json) | The counts: covers by status, by theme and by decade |
| [years/2005.json](api/years/2005.json) | One year per file, from [years/2000.json](api/years/2000.json) to [years/2026.json](api/years/2026.json) |

## One record looks like this

```json
{
  "year": 2005,
  "date": "June 18, 2005",
  "cover": "After the fall",
  "theme": "Money and markets",
  "prediction": "The world housing bubble, the biggest in history, would pop",
  "status": "happened",
  "status_label": "✅ HAPPENED",
  "what_happened": "US house prices fell by about a third and helped cause the 2008 financial crisis.",
  "page": "https://aamirtechs.github.io/economist-front-page-explained/years/2005.html"
}
```

## The status values

- `happened`: events matched what the cover said or warned
- `partly_happened`: part of it happened, or it happened for a different reason
- `did_not_happen`: events went the other way
- `not_a_prediction`: a judgment, a portrait or a report, not a forecast
- `pending`: too early to tell, the story belongs to the future

## Rules of use

The explanations, verdicts and data structure are this project's own work, written from the public record. The cover artwork and headlines belong to The Economist, and this API does not include any cover images. If you build something with the data, a link back to this site is appreciated.
