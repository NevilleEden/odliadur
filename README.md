# Odliadur

A small Welsh end-rhyme finder. Type an ending (for example `ydd`) and it lists every word in the word list that ends that way. Tap a word to see its bundled meaning or open it in Geiriadur Prifysgol Cymru.

This is a personal tool inspired by the book *Yr Odliadur*. It contains no text from that book.

## Files

- `index.html` - the whole app (no build step)
- `words.json` - the word list (about 81,000 words)
- `meanings.json` - short English meanings (about 15,000 words) taken from Wiktionary, plus plural/inflected forms pointing to their base word
- `meanings-extra.json` - about 4,300 more meanings from the Apertium/Eurfa Welsh-English data
- `icon.svg`, `apple-touch-icon.png`, `favicon-32.png`, `icon-192.png`, `icon-512.png` - app icons

## Credits and licences

- Word list: Welsh spelling dictionary from Bangor University's Language Technologies Unit (Uned Technolegau Iaith) and Troi, licensed under the GNU LGPL v3 or later. Source: https://github.com/techiaith/hunspell-cy . `words.json` is derived from that dictionary (cleaned, with regular plural endings added).
- Meanings (`meanings.json`): Welsh entries from Wiktionary, extracted with kaikki.org (wiktextract), available under CC BY-SA 4.0 (https://creativecommons.org/licenses/by-sa/4.0/). The file is a shortened adaptation and is shared under the same licence.
- Meanings (`meanings-extra.json`): derived from the Welsh-English bilingual dictionary of the Apertium project (https://github.com/apertium/apertium-cy-en, by Kevin Donnelly and others, based on Eurfa), licensed under the GNU GPL v2 (see `LICENSE-GPL-2.0.txt`). Source data: the file `apertium-cym-eng.cym-eng.dix` in that repository.
- The page makes no live lookups. Tapping a word shows the bundled meaning (if any) and a link to Geiriadur Prifysgol Cymru.
- Inspired by *Yr Odliadur* by Roy Stephens and Alan Llwyd (ISBN 978-1-84323-903-1). Independent and not affiliated with the authors or publisher.

## Known limitations

- It matches the letters at the end of a word. It does not yet separate the two different *wy* sounds, and it does not apply the foreword's rules about which vowels rhyme across *y*, *u* and *i*.
- Only about a quarter of the words have a bundled meaning. Many are rare, compound or inflected verb forms that the open dictionaries do not cover.
- Some Wiktionary glosses are brief or technical; check anything important in Geiriadur Prifysgol Cymru.
- Verb forms are included only where the source dictionary lists them as separate entries.
