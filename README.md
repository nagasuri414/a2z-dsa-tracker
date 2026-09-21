# A2Z DSA Tracker

An unofficial, browser-based practice tracker built around [Striver's A2Z DSA sheet](https://takeuforward.org/dsa/strivers-a2z-sheet-learn-dsa-a-to-z). It is not affiliated with takeUforward. Problem, article, and video links point to their original providers.

## Use it

Open `index.html` in a browser, or publish that file with GitHub Pages. Ticks, notes, stars, and goals are stored in that browser; they are **not** saved to GitHub or shared with other users. Use **Data → Download backup (.json)** regularly, and **Restore backup (.json)** when moving to another browser or computer. The Excel and CSV files are standalone sheet exports.

Before replacing a local download with a new version, download a JSON backup. Browser storage for pages opened directly from the filesystem can vary by browser and file location.

The **AI** button opens a ready-made prompt for that problem — intuition, complexity, and C++ code — in whichever assistant you pick from **Ask AI** in the toolbar (ChatGPT, Claude, or Gemini; ChatGPT is the default because it's the only one of the three confirmed to open straight into an answer — Claude and Gemini open the site with the prompt already on your clipboard, ready to paste). This app has no connection to any of them and stores nothing about what you ask.

Clicking a problem's name expands a quick summary — step, topic, difficulty, and your own note. A small, hand-verified set of problems (compiled and cross-checked before being added, listed in the commit history) also show a trick, complexity, and working code directly, no AI needed.

## Repository contents

This repository shares the ready-to-use `index.html`, Excel workbook, and CSV export. The development materials in `reference/`, your personal progress in `personal/`, and the notes PDF remain only on the maintainer's computer. The browser app is self-contained in `index.html`; no build step is needed to use it.
