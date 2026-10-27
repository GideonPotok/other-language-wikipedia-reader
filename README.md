# Other-language Wikipedia reader

A single-page reader for Hebrew Wikipedia in English. Search in English or Hebrew, read a machine translation with tap-to-reveal originals, and compare the Hebrew and English articles section by section.

Live: https://gideonpotok.github.io/other-language-wikipedia-reader/

- No build, no dependencies: `index.html` is the whole app.
- Article text comes from the Wikipedia Action API (`he.wikipedia.org`, `en.wikipedia.org`), CC BY-SA 4.0.
- Translation runs through a chain of providers: Google's free endpoint, Google's dictionary endpoint, then MyMemory. A provider that fails or rate-limits is rested for a while and the next one takes the batch. Under **Translators** you can add a Claude API key (best quality; can be set to go first) or a Google Cloud Translation key; keys stay in the browser's localStorage.
- Translations, font size and view mode are cached in the browser's localStorage.
