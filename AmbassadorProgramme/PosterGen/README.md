# PosterGen

All code and assets for generating and improving the workshop poster live here.

## Contents

- **poster.html** – Workshop poster (Generative AI Agent 101). Open in a browser or use `npm run screenshot` to export `poster.jpg`.
- **prepPoster.md** – Brief and requirements used to create the poster.
- **setupNano.md** – Instructions to use Poe (e.g. Nano-Banana-Pro) to generate improvement suggestions.
- **screenshot-poster.js** – Puppeteer script to capture the poster as a JPG.
- **genBetterPoster.js** – Calls Poe API to analyze `poster.html` and write **betterPoster.md** (summary + suggestions + optional revised copy).

## Setup

1. **Dependencies** (from this folder):
   ```bash
   cd AmbassadorProgramme/PosterGen && npm install
   ```

2. **Poe API key** (for `npm run better`):
   - Create `AmbassadorProgramme/LLM/poeKey.md` and put your Poe API key on the first line.
   - See `AmbassadorProgramme/LLM/dummyPoe.md` for full instructions.

## Commands

From `AmbassadorProgramme/PosterGen`:

- **Export poster as JPG:**  
  `npm run screenshot`  
  Writes `poster.jpg` in this folder.

- **Generate betterPoster.md via Poe:**  
  `npm run better`  
  Uses the key in `../LLM/poeKey.md` and the Poe model set in `POE_POSTER_MODEL` (default: `Nano-Banana-Pro`). To use a different model, e.g. Claude:  
  `POE_POSTER_MODEL=Claude-Sonnet-4 npm run better`

## Moved from

Poster-related files were moved here from `AmbassadorProgramme/` as per `setupNano.md`.
