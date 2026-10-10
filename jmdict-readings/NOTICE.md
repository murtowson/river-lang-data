# jmdict-readings — Japanese word readings

**Source:** JMdict (JMdict_e.gz) by the Electronic Dictionary Research and Development Group (EDRDG), https://www.edrdg.org/jmdict/j_jmdict.html

**License:** CC BY-SA 4.0 — `../LICENSES/CC-BY-SA-4.0.txt`, together with the EDRDG licence statement https://www.edrdg.org/edrdg/licence.html. This modified file is distributed under the same license.

**What was changed and when (River Lang):** only written forms and their kana readings were kept (SQLite `readings(k, v)`: written form → comma-separated kana readings), everything else (glosses, tags) was dropped; XML parsed without external entities. 2026-10-09: gzip.

The conversion is fully described above; the build script lives in the (private) app repository.
