# Fixate

A self-contained RSVP (rapid serial visual presentation) speed-reading app. No build step, no dependencies, no server — the whole app, a 61-book library, and a built-in dictionary are baked into single HTML files.

**Live app:** https://rekursivestudios.github.io/fixate/ (the Full library build, below)

## Reading modes

- **Flash** — the classic RSVP mode, one word (or chunk of words) at a time, replacing in place
- **Glide** — words slide to a fixed anchor point instead of cross-fading
- **Flow** — continuous horizontal scroll, with the focus word dimmed less than its neighbors
- **Rise** — continuous vertical scroll, same idea as Flow but top-to-bottom or bottom-to-top
- **Split** — alternates words left/right, one per eye
- **Trio** — full stream down the center, with recent words echoed to both sides

Plus a built-in dictionary (hover or Alt-click any word for a definition, related words, and a breadcrumb trail), real page counts recovered from the original printed editions where available, and an optional text-to-speech voice that reads along as each word comes into focus.

## Downloads

| File | Contents | Size |
|---|---|---|
| [`index.html`](index.html) | 58 books + 3 samples + dictionary (this is the live site above) | ~24.5 MB |
| [`full-library-no-dictionary.html`](full-library-no-dictionary.html) | Same 58 books, no dictionary lookup (smaller) | ~19.6 MB |
| [`fiction.html`](fiction.html) | Fiction shelf only | ~15.0 MB |
| [`philosophy-religion.html`](philosophy-religion.html) | Philosophy & Religion shelf only | ~9.6 MB |
| [`politics-economics.html`](politics-economics.html) | Politics & Economics shelf only | ~6.7 MB |
| [`ingersoll.html`](ingersoll.html) | Robert Ingersoll shelf only | ~10.0 MB |
| [`app-only.html`](app-only.html) | Just the 3 original sample texts, no library | ~5.6 MB |

Each file is the entire app — open it in any browser, online or off. Download one and open it locally if you'd rather not depend on this page being up, or if you want it stored as a plain file on your phone.

## Why single-file HTML

Built to work fully offline, including from a downloaded file opened directly on a phone (no app store, no install). That environment can't reliably use browser storage, so everything — the library, the dictionary, your settings — either ships baked into the file itself or exports/imports as a small `.wv` settings file you keep alongside it.

Opened from this GitHub Pages site instead of a downloaded file, the app also gets real persistent settings (your last position, custom presets) since it's served over `https://` rather than opened as a local file.

## Credits

- All 61 books are public domain (Project Gutenberg) or original texts written for this app.
- The built-in dictionary is derived from Webster's Revised Unabridged Dictionary (1913), via the [matthewreagan/WebstersEnglishDictionary](https://github.com/matthewreagan/WebstersEnglishDictionary) public-domain dataset.
- Sukashi, the included typeface, is a Rekursive Studios original.
