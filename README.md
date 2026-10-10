# River Lang — open data

This repository contains the **processed data files** that the language-learning app
**River Lang** downloads on demand: dictionaries, character data and stroke order.
The app's source code is not here and is not covered by these licenses — the app only
*reads* these files.

Each dataset keeps the license of its source. Where the license requires it
(Arphic Public License, CC BY-SA, LGPL), the **modified files are published here in full**,
with a `NOTICE.md` in every folder saying what was changed and when. Nothing here is
original work of River Lang except the conversion; the credit belongs to the authors below.

## Datasets

| folder | source | author | license |
|---|---|---|---|
| `cedict/` | CC-CEDICT — https://www.mdbg.net/chinese/dictionary?page=cc-cedict | MDBG and contributors | CC BY-SA 4.0 |
| `cfdict/` | CFDICT — chine.in | CFDICT contributors | CC BY-SA 3.0 |
| `handedict/` | HanDeDict — https://handedict.zydeo.net | HanDeDict contributors | CC BY-SA 3.0 |
| `jmdict-readings/` | JMdict — https://www.edrdg.org/jmdict/j_jmdict.html | Electronic Dictionary Research and Development Group | CC BY-SA 4.0 + EDRDG licence |
| `strokes-zh/` | Make Me a Hanzi `graphics.txt` via hanzi-writer-data 2.0.1 — https://github.com/skishore/makemeahanzi | Shaunak Kishore; glyphs from Arphic PL KaitiM GB and Arphic PL UKai (c) 1999 Arphic Technology | Arphic Public License |
| `decomposition-zh/` | Make Me a Hanzi `dictionary.txt` | Shaunak Kishore (from Unihan and CJKlib) | LGPL-3.0-or-later |
| `examples/` | Tatoeba — https://tatoeba.org | sentence authors, named for every sentence | CC BY 2.0 FR |
| `unihan/` | Unihan Database, Unicode 18.0 — https://www.unicode.org/charts/unihan.html | Unicode, Inc. | Unicode License v3 |

Full license texts are in `LICENSES/`. Every folder has `NOTICE.md` (source, version,
changes) and `SHA256SUMS`; the app checks the SHA-256 of every file it downloads.

Files are SQLite databases, gzip-compressed (`.db.gz`).

## Attribution (as shown in the app, Settings → Licenses)

- CC-CEDICT, CC BY-SA 4.0 (modified).
- CFDICT and HanDeDict, CC BY-SA 3.0 (modified).
- JMdict, © EDRDG, CC BY-SA 4.0 (modified).
- Stroke order data: Make Me a Hanzi (Shaunak Kishore), derived from Arphic PL KaitiM GB and
  Arphic PL UKai fonts (c) 1999 Arphic Technology Co., Ltd. — Arphic Public License.
- Character decomposition: Make Me a Hanzi, LGPL-3.0-or-later.
- Example sentences: Tatoeba (https://tatoeba.org), CC BY 2.0 FR — the author is shown with every sentence.
- Unihan Database (c) Unicode, Inc., Unicode License v3.

## Not legal advice

The summaries above are for orientation; the license texts in `LICENSES/` are authoritative.
