# cedict — Chinese–English dictionary, readings grouped

**Source:** CC-CEDICT by MDBG and contributors, https://www.mdbg.net/chinese/dictionary?page=cc-cedict — release of 2026-10-01T07:35:40Z, 125,163 entries.

**License:** CC BY-SA 4.0 — `../LICENSES/CC-BY-SA-4.0.txt`. This modified file is distributed under the same license.

**What was changed and when (River Lang):** 2026-10-02: comment lines dropped; numbered pinyin converted to tone marks (`xing2` → `xíng`); stored in SQLite `entries(simp, trad, py, glosses)` with indexes on simp and trad, plus `meta`. No gloss was changed. 2026-10-09: gzip (level 9, no name, no time) — this is what the app downloads.

The conversion is fully described above; the build script lives in the (private) app repository.
