# unihan — extract of the Unihan Database (Chinese)

**Source:** Unicode 18.0.0 `Unihan.zip` (SHA-256 `4c93ea9c1f636451729a840978f1667a53886af37ba854fdcce109721c63d43e`) and `CJKRadicals.txt`
(SHA-256 `689e2e5852699e7115823dc0b6d3e615eb767c7f477b615678f4f989d1f06105`), https://www.unicode.org/Public/18.0.0/ucd/

© 1991-2026 Unicode, Inc. **License:** Unicode License v3 — `LICENSES/UNICODE-LICENSE-V3.txt`.

**What was extracted (2026-10-09, River Lang):** for every character that has `kMandarin` or
`kDefinition` (45496 characters) — `kDefinition`, `kMandarin`, `kTotalStrokes` (first value,
zh-Hans), `kRSUnicode` (first value; the radical number is mapped to its unified ideograph with
`CJKRadicals.txt`, e.g. `120.11` → 糸 + 11, `120'.4` → 纟 + 4), `kSimplifiedVariant` and
`kTraditionalVariant` (as characters). SQLite table `chars(ch, def, mandarin, strokes, rad,
rad_num, rad_extra, simp, trad)` plus `meta`; gzip (level 9, no name, no time).

The conversion is fully described above; the build script lives in the (private) app repository.

License texts: `../LICENSES/UNICODE-LICENSE-V3.txt`
