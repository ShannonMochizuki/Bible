# Journey Through Joshua

A modular, game-like Bible study PWA. Version 1 contains Joshua 1–4 and is designed for use alongside the NKJV.

## Included
- Multiple local profiles
- Joshua journey map and chapter hub
- Joshua 1–4 content modules
- Observation / understanding / connection questions
- Multiple-choice, multi-select, and ordering interactions
- “Show me in Scripture” evidence references
- Insights and discoveries collection
- Ungraded chapter reflection journal
- Spaced-repetition review queue
- Memory-passage list
- Local persistence with `localStorage`
- Installable/offline PWA shell

## NKJV note
The New King James Version is copyrighted by Thomas Nelson. This repository does not reproduce the full NKJV text. It references exact NKJV passages and is architected so licensed verse text can later be connected as a content provider.

## Run locally
Serve the folder with any static web server, for example:

```bash
python -m http.server 8080
```

Then visit `http://localhost:8080`.

## Content architecture
Joshua content is isolated in `content/joshua.js`. Additional books can follow the same shape without rebuilding the UI engine.
