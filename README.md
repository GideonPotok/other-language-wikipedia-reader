# Other-language Wikipedia reader

A single-page reader for Hebrew Wikipedia in English. Search in English or Hebrew, read a machine translation with tap-to-reveal originals, and compare the Hebrew and English articles section by section.

Live: https://gideonpotok.github.io/other-language-wikipedia-reader/

- No build, no dependencies: `index.html` is the whole app.
- Article text comes from the Wikipedia Action API (`he.wikipedia.org`, `en.wikipedia.org`), CC BY-SA 4.0.
- Translation uses Google Translate's public `translate_a/single` endpoint (unofficial, keyless). If it is unreachable the page falls back to Hebrew.
- Translations, font size and view mode are cached in the browser's localStorage.
