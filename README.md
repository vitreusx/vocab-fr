# Vocab FR

A single-page French vocabulary tool. Look up a word, get definitions from Wiktionary (English + French), and add it as an Anki flashcard directly from your browser.

## Setup

### 1. Install AnkiDroid + AnkiConnect Android

- Install [AnkiDroid](https://play.google.com/store/apps/details?id=com.ichi2.anki) from the Play Store.
- Install [AnkiConnect Android](https://github.com/KamWithK/AnkiconnectAndroid) — sideload the APK from its GitHub releases page.
- Enable the add-on inside AnkiDroid: **Settings → Advanced → Enable AnkiConnect**.
- Keep AnkiDroid running in the background whenever you use the app.

### 2. Create the deck

AnkiConnect Android won't create decks automatically. Before adding your first card, open AnkiDroid and create a deck named **Vocab FR** (or whatever name you plan to use in the app).

### 3. Configure the CORS host

By default AnkiConnect Android only accepts requests from the same origin. You need to whitelist the URL you'll be loading the app from.

In AnkiDroid: **Settings → Advanced → AnkiConnect → CORS host**

Enter the origin of the page, e.g.:

- `https://vitreusx.github.com/vocab-fr` — Default, using GH Pages.
- `http://10.0.2.2:8080` — Android emulator (for debugging purposes.)

## Debugging

Open `index.html` in Chrome (or serve it with `python3 -m http.server 8080` and navigate to the URL). Type a French word, hit **Chercher**, then tap **Ajouter la carte** to push it to AnkiDroid.
