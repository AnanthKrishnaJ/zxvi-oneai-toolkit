# ZXVI OneAI Toolkit

A single-file, **fully offline** toolkit with **175 tools** – no API keys, no servers, no accounts, no tracking. Everything runs in the browser.

- **Mobile-app style UI** that becomes a true full-window desktop workspace on wide screens
- **Smart search** – type what you want to do ("shrink a photo", "solve a sudoku from a picture") and it finds the tool
- **40 colour themes** (plus light / dark / system), saved on the device
- **Word Search solver** – type or *scan a photo of a puzzle* (offline OCR), then reveal answers one by one or print the solved sheet
- **Sudoku** – play, generate, type your own, or *scan a photo* and solve it step by step
- **Image to Story** – drop in a picture and get a story built from its colours, light and mood (template based, works offline – it does not "recognise" objects, so add a hint for better stories)
- **Profile** – name, username, bio, emoji / photo avatar, accent colour, export / import backup (stored in the browser)

## Run locally
Open `index.html` in a browser, or serve the folder: `npx serve .`

## Deploy to Vercel
1. Import this GitHub repo at <https://vercel.com/new> (Framework preset: **Other**, no build command, output directory = root).
2. Or from a terminal: `npm i -g vercel && vercel --prod`.

## Project layout
| File | Purpose |
|---|---|
| `index.html` | The whole app (HTML + CSS + JS) |
| `vercel.json` | Static hosting settings |

## Known limits
- Photo scanning is template-matching OCR: clean, straight, printed grids work best; tiny thin text, heavy skew (>10°) or curved photos may need the manual edit step.
- Printing from some embedded previews can be blocked by the browser – open the page directly.
