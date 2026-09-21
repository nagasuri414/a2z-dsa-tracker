# A2Z DSA Tracker

An unofficial, browser-based practice tracker built around [Striver's A2Z DSA sheet](https://takeuforward.org/dsa/strivers-a2z-sheet-learn-dsa-a-to-z). It is not affiliated with takeUforward. Problem, article, and video links point to their original providers.

## Use it

Open `index.html` in a browser alongside `quotes.js` and `solutions.js`, or publish all three with GitHub Pages. Ticks, notes, stars, and goals are stored in that browser; they are **not** saved to GitHub or shared with other users. Use **Data → Download backup (.json)** regularly, and **Restore backup (.json)** when moving to another browser or computer. The Excel and CSV files are standalone sheet exports.

Before replacing a local download with a new version, download a JSON backup. Browser storage for pages opened directly from the filesystem can vary by browser and file location.

The **AI** button opens a ready-made prompt for that problem — intuition, complexity, and C++ code — in whichever assistant you pick from **Ask AI** in the toolbar (ChatGPT, Claude, or Gemini; ChatGPT is the default because it's the only one of the three confirmed to open straight into an answer — Claude and Gemini open the site with the prompt already on your clipboard, ready to paste). This app has no connection to any of them and stores nothing about what you ask.

Clicking a problem's name expands a quick summary — step, topic, difficulty, and your own note. All 456 roadmap items have a quick solution with an approach, time/space complexity, and C++ code. Introductory theory lessons use illustrative C++ examples rather than a judge-specific submission.

## Repository contents

This repository shares the ready-to-use `index.html`, `quotes.js`, `solutions.js`, 18 editable `solutions/step-XX.json` files, Excel workbook, and CSV export. The browser reads the single generated `solutions.js` file; the step files are its source. After editing a step file, regenerate the master with `python3 reference/scripts/build_solutions.py` on the maintainer's machine. Development materials in `reference/`, personal progress in `personal/`, and the notes PDF remain local. No build step is needed to use the published page.
