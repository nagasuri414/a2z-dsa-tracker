# A2Z DSA Tracker

**Live: [nagasuri414.github.io/a2z-dsa-tracker](https://nagasuri414.github.io/a2z-dsa-tracker/)**

An unofficial, browser-based practice tracker built around [Striver's A2Z DSA sheet](https://takeuforward.org/dsa/strivers-a2z-sheet-learn-dsa-a-to-z) — 456 problems across 18 steps, with links to GFG/LeetCode/YouTube/etc., space for your own notes, and a quick solution for almost every problem. It is not affiliated with takeUforward; problem, article, and video links point to their original providers.

## Using it

Open the live link above — nothing to install, no account needed. The page itself has a **How to use** button in the top toolbar with the same walkthrough below, and it opens automatically the first time you visit.

- **Your progress saves in that browser only.** It is not synced anywhere or shared with anyone else who opens the same link — everyone gets their own, separate, private progress. This is the one thing worth understanding up front, since it surprises people: clearing your browser's data, or opening the link on a different device, starts fresh unless you've backed up.
- Use **Save & load → Download backup (.json)** every so often to keep an external copy, and **Restore backup (.json)** to bring it back on another browser or device. On desktop Chrome/Edge, **Save & load → Autosave to a file** connects a local JSON file that is updated continuously instead. Storage status and backup controls also appear at the bottom of the tracker.
- Tick the checkbox to mark a problem solved; the star and note icons sit next to it.
- The **AI** link opens a ready-made prompt explaining that problem — intuition, complexity, and C++ code — in whichever assistant you pick from **Ask AI** in the toolbar (ChatGPT, Claude, or Gemini; ChatGPT is the default because it's the only one of the three confirmed to open straight into an answer — Claude and Gemini open the site with the prompt already on your clipboard, ready to paste). This app has no connection to any of them and stores nothing about what you ask.
- The `</>` icon shows a quick solution — approach, time/space complexity, and C++ code — for almost every problem. Introductory theory lessons use illustrative C++ examples rather than a judge-specific submission. Only a small, original set of these was individually compiled and cross-checked against brute-force references before being added (see the commit history); the rest were integrated without that same verification pass, so treat any solution as a starting point to check, not a guaranteed-correct answer key.
- **Save & load** can also export/import your progress as an Excel workbook, including a progress-by-step chart and dropdown-assisted editable cells, if you'd rather track things there.
- Search, filters, dark mode, and the collapsible progress report (daily activity, pace toward a goal) are worth exploring too.

## Repository contents

This repository shares the ready-to-use `index.html`, `quotes.js`, `solutions.js`, 18 editable `solutions/step-XX.json` files, an Excel workbook, and a CSV export. The browser reads the single generated `solutions.js` file; the step files are its source. After editing a step file, regenerate it with `python3 reference/scripts/build_solutions.py` on the maintainer's machine. Development materials in `reference/`, personal progress in `personal/`, and the notes PDF remain local. No build step is needed to use the published page.

Running it from a local download instead of the live link works the same way, opening `index.html` alongside `quotes.js` and `solutions.js` in a browser — but download a JSON backup before replacing a local copy with a newer one, since browser storage for pages opened directly from the filesystem can behave differently depending on the browser and where the files sit on disk.
