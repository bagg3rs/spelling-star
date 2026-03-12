# Spelling Star ⭐ — Backlog

## Live ✅
- [x] Spelling test mode (type to check, 3 attempts, hints)
- [x] British English text-to-speech (hear the word)
- [x] Stars, streaks, confetti, best score tracking
- [x] Parent word list input (one per line, saved to localStorage)
- [x] Write-before-type mode (canvas drawing step before typing)
- [x] Pen colour picker (7 colours)
- [x] Letter practice mode (a-z grid, guide letter, formation instructions)
- [x] Handwriting scoring (pixel overlap: coverage + precision bars, personal bests)

## Backlog 📋

### Next Up
- [ ] **📸 Photo OCR word import** — take photo of homework sheet, OCR extracts spelling list automatically
- [ ] **💾 Progress tracking** — save scores over time, show improvement graph per week
- [ ] **🤖 AI handwriting feedback** (Phase 2) — serverless function sends canvas to vision model, returns kid-friendly formation tips ("your tail needs to curl more")

### Future Ideas
- [ ] Multiple word lists (save/name different weeks: "Week 12", "Week 13")
- [ ] Parent dashboard (see all scores, which words are tricky, which letters need practice)
- [ ] Reward system / unlockables (new pen colours, backgrounds earned through practice)
- [ ] Maths mode (addition/subtraction challenges at Year 1 level)
- [ ] Reading mode (show word → say it out loud → mic check?)
- [ ] Timed challenge mode (how many in 60 seconds)
- [ ] PWA / Add to Home Screen with icon
- [ ] Custom domain (spelling.onelumen.co.uk or similar)

## Tech Notes
- **Repo:** https://github.com/bagg3rs/spelling-star
- **Live:** https://bagg3rs.github.io/spelling-star/
- **Stack:** Single HTML file, no dependencies, GitHub Pages
- **Data:** All client-side localStorage (no backend yet)
- **OCR options:** Tesseract.js (client-side, ~2MB WASM) or serverless + cloud vision API
- **AI scoring:** Cloudflare Worker → vision model API (keeps API keys server-side)
