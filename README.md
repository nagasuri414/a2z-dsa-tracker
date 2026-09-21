# A2Z DSA Tracker

An unofficial, browser-based practice tracker built around [Striver's A2Z DSA sheet](https://takeuforward.org/dsa/strivers-a2z-sheet-learn-dsa-a-to-z). It is not affiliated with takeUforward. Problem, article, and video links point to their original providers.

## Use it

Open `index.html` in a browser, or publish that file with GitHub Pages. Ticks, notes, stars, and goals are stored in that browser; they are **not** saved to GitHub or shared with other users. Use **Data → Download backup (.json)** regularly, and **Restore backup (.json)** when moving to another browser or computer. The Excel and CSV files are standalone sheet exports.

Before replacing a local download with a new version, download a JSON backup. Browser storage for pages opened directly from the filesystem can vary by browser and file location.

The **AI** button opens a live ChatGPT conversation with a ready-made prompt for that problem — intuition, complexity, and code in three languages. It works if you already have ChatGPT open in your browser; the prompt is also copied to your clipboard as a fallback, and can be pasted into any other assistant. This app has no connection to OpenAI and stores nothing about what you ask.

## Repository contents

This repository shares the ready-to-use `index.html`, Excel workbook, and CSV export. The development materials in `reference/`, your personal progress in `personal/`, and the notes PDF remain only on the maintainer's computer. The browser app is self-contained in `index.html`; no build step is needed to use it.
