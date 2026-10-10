# strokes-zh — Chinese stroke order data

**Source:** hanzi-writer-data 2.0.1 (npm, tarball SHA-256 `72baf3d82b114e60d6e40ea05f24d2262a05cd39d544e2f322ba2fceb7beff15`), which is the
per-character split of Make Me a Hanzi `graphics.txt`
(https://github.com/skishore/makemeahanzi) by Shaunak Kishore, prepared by David Chanin.

**Original glyphs:** Arphic PL KaitiM GB and Arphic PL UKai © 1999 Arphic Technology Co., Ltd.

**License:** Arphic Public License — `LICENSES/ARPHICPL.TXT` (full text).

**What was changed and when (2026-10-09, River Lang):**

- the per-character JSON files (`strokes`, `medians`, `radStrokes`) were packed **unchanged,
  byte for byte** into SQLite: table `strokes(ch TEXT PRIMARY KEY, data TEXT)`, plus `meta`
  (source, license, this notice);
- split into two files: `strokes-zh-common-v1` — the 3,500 characters of 通用规范汉字表 (2013)
  level 1 (list: shengdoushi/common-standard-chinese-characters-table@d9b599a9c9cc0dd2d58cad829e285bc780cd4451, `level-1.txt`,
  SHA-256 `79a6c710013cc86617d5db65871f59b2d67dee72415d380a2cc7145a51450fe4`); `strokes-zh-rare-v1` — the other 6074 characters;
- gzip (level 9, no name, no time) — this is what the app downloads.

No stroke outline, median or radical index was altered. Note: hanzi-writer-data 2.0.1 was
published in 2018; later fixes in Make Me a Hanzi `graphics.txt` may be missing (not checked).

The conversion is fully described above; the build script lives in the (private) app repository.

License texts: `../LICENSES/ARPHICPL.TXT`
