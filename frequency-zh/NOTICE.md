# frequency-zh — Chinese word frequency ranks

**Source:** jieba `dict.txt` at commit `67fa2e36e72f69d9134b8a1037b83fbb070b9775`
(https://github.com/fxsjy/jieba/blob/67fa2e36e72f69d9134b8a1037b83fbb070b9775/jieba/dict.txt, SHA-256 `7197c3211ddd98962b036cdf40324d1ea2bfaa12bd028e68faa70111a88e12a8`),
by Sun Junyi.

**License:** MIT License, Copyright (c) 2013 Sun Junyi — `LICENSES/MIT-jieba.txt` (full text,
from the same commit, SHA-256 `18ba0984839f85853b29fadaf992f7dba8fd0ca0fbeae34de2b8735222dc7a37`).

**What was changed and when (2026-10-10, River Lang):**

- kept only words that are also headwords of CC-CEDICT, simplified or traditional
  (88,474 of 349,045 jieba words);
- the frequency count was replaced by its **rank** among the kept words: 1 = most frequent,
  equal counts share a rank (1 + the number of kept words with a higher count);
- part-of-speech tags dropped;
- stored in SQLite: table `freq(word TEXT PRIMARY KEY, rank INTEGER)`, plus `meta` (source,
  license, this notice);
- gzip (level 9, no name, no time) — this is what the app downloads.

Used by the River Lang dictionary search to put frequent words first (e.g. `fanrong` → 繁荣
before 烦冗). Build script: `scripts/build-freq-pack.py` in the River Lang app repository.

License text: `../LICENSES/MIT-jieba.txt`
