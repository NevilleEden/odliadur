# Odliadur

A small Welsh end-rhyme finder. Type an ending (for example `ydd`) and it lists every word in the word list that ends that way. Tap a word to see its meaning (fetched live from Wiktionary) or open it in Geiriadur Prifysgol Cymru.

This is a personal tool inspired by the book *Yr Odliadur*. It contains no text from that book.

## Files

- `index.html` - the whole app (no build step)
- `words.json` - the word list (about 81,000 words)

## Credits and licences

- Word list: Welsh spelling dictionary from Bangor University's Language Technologies Unit (Uned Technolegau Iaith) and Troi, licensed under the GNU LGPL v3 or later. Source: https://github.com/techiaith/hunspell-cy . `words.json` is derived from that dictionary (cleaned, with regular plural endings added).
- Meanings: fetched live from Wiktionary, available under CC BY-SA 4.0.

## Known limitations

- It matches the letters at the end of a word. It does not yet separate the two different *wy* sounds, and it does not apply the foreword's rules about which vowels rhyme across *y*, *u* and *i*.
- The word list has no part-of-speech labels.
- Verb forms are included only where the source dictionary lists them as separate entries.
