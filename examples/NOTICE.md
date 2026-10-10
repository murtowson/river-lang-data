# examples — Chinese example sentences from Tatoeba

`tatoeba-zh-v1.db.gz` is a selection from the Tatoeba corpus (https://tatoeba.org):
Mandarin (cmn) sentences that have an English and/or Russian translation, plus a
word → sentences index.

## License

Tatoeba sentences are licensed under **Creative Commons Attribution 2.0 France
(CC BY 2.0 FR)** — `../LICENSES/CC-BY-2.0-FR.txt`,
https://creativecommons.org/licenses/by/2.0/fr/ ; some sentences are CC0 1.0
(marked `cc0 = 1` in the file). Tatoeba terms: https://tatoeba.org/en/terms_of_use

**The author of every sentence and of every translation** is kept in the file
(table `authors`, field `author`) — the Tatoeba user who owned the sentence on the
export date. The app shows it under every example ("Tatoeba · author · CC BY").
The sentence number (`id`) leads to https://tatoeba.org/sentences/show/<id>.
Sentences without a known owner were not included.

## What was changed (2026-10-09, River Lang)

Sentences up to 60 characters with a translation were selected; at most one
translation per language (with an author, the earliest). **Sentence texts were not
edited.** The word index was built with the segmentit segmenter (MIT) plus CC-CEDICT
headwords. This selection is a derivative work and is distributed under the same
license (CC BY 2.0 FR).

## Source

Tatoeba export of Sat, 03 Oct 2026 06:29:49 GMT
(`downloads.tatoeba.org/exports/per_language/`); file names, sizes and SHA-256 of
every input are in `MANIFEST.json`, counts in `stats.json`.

66,219 sentences; 63,649 with an English translation, 10,030 with a Russian one;
28,761 indexed words; 2,743 authors.

The conversion is fully described above; the build script lives in the (private) app repository.
