# decomposition-zh — what Chinese characters are made of

**Source:** Make Me a Hanzi `dictionary.txt` at commit `bddc96d41bef78427ed0e034e9f7e31d71fd1b92`
(https://github.com/skishore/makemeahanzi, SHA-256 `744bb05d5b0742e9ee35c37791f94d56a173349b3367569e7ca11e510364d203`), by Shaunak Kishore,
derived from Unihan and CJKlib.

**License:** GNU LGPL-3.0-or-later — `LICENSES/LGPL-3.0.txt` (and `GPL-3.0.txt`, which it
incorporates).

**What was changed and when (2026-10-09, River Lang):**

- kept the fields `character`, `decomposition`, `radical`, `etymology`; dropped `definition`,
  `pinyin`, `matches`. Values are unchanged;
- stored in SQLite: table `decomp(ch TEXT PRIMARY KEY, decomposition TEXT, radical TEXT,
  etymology TEXT)` (etymology as compact JSON), plus `meta` with this notice; 9574 characters;
- gzip (level 9, no name, no time) — this is what the app downloads.

The original `dictionary.txt` is available from the source above; the modified file is here.
The conversion is fully described above; the build script lives in the (private) app repository.

License texts: `../LICENSES/LGPL-3.0.txt`, `../LICENSES/GPL-3.0.txt`
