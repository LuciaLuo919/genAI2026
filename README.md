# genAI2026

AI ambassador programme at HKBU.

## Repository structure

| Folder | Contents |
|--------|----------|
| **[courses/](./courses/)** | Course materials (UCLC1008, GCAP3056). Includes AIagentDemo, lessons, materials, Moodle posts. |
| **[AmbassadorProgramme/](./AmbassadorProgramme/)** | AI ambassador programme drafts and revised messages. |
| **[replit/](./replit/)** | Web app (Vite + React + Express). Moved from repo root for deployment. |
| **[issues/](./issues/)** | Issue tracking. |

## Running the project

- **Locally:** `cd replit && npm install && npm run dev`
- **On Replit:** See [replit/REPLIT.md](./replit/REPLIT.md) for the live link and setup.

## Publishing all HTML (GitHub Pages)

To serve all HTML and static files from this repo:

1. **GitHub** → **Settings** → **Pages**.
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
3. Choose **Branch:** `main`, **Folder:** `/ (root)`. Save.
4. The repo has a **`.nojekyll`** file at root so Jekyll is disabled and every file (including all `.html`) is served as-is.

Base URL: **https://tesolchina.github.io/genAI2026/**  
Example HTML: `courses/UCLC1008/AIagentDemo/teacherJumpIntoWater/guide_game_FRT.html` →  
https://tesolchina.github.io/genAI2026/courses/UCLC1008/AIagentDemo/teacherJumpIntoWater/guide_game_FRT.html
