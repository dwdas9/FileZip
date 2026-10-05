FileZip — Third-Party Notices
=============================

FileZip includes one third-party component: the 7-Zip command-line engine.

7-Zip 26.03 (`7zz`)
-------------------

- Copyright (C) 1999-2026 Igor Pavlov.
- Website: https://www.7-zip.org/
- Source used for this build:
  https://github.com/ip7z/7zip/releases/download/26.03/7z2603-src.tar.xz
  (SHA-256 9cbde5099c6deb73691b0579063da5827522ccbbcba3f0020fd04e8c8c16c0d4)
- Location in the app: `FileZip.app/Contents/MacOS/7zz`

Licenses that apply to the code included in FileZip's build:

- **GNU Lesser General Public License, version 2.1 or later** — most of 7-Zip.
  Full text: `licenses/GNU-LGPL-2.1.txt` (in the app: `Contents/Resources/Licenses/GNU-LGPL-2.1.txt`).
- **BSD 3-clause License** — LZFSE decompression (derived from Apple's LZFSE
  library, Copyright (c) 2015-2016 Apple Inc.) and ZSTD decompression (developed
  with reference to the zstd decoder, Copyright (c) Facebook, Inc.).
- **BSD 2-clause License** — XXH64 hashing (`C/Xxh64.c`).
- Some files are in the public domain, as stated in those files.

The complete 7-Zip license file, including the full BSD license texts, is in
`licenses/7-Zip-License.txt` (in the app: `Contents/Resources/Licenses/7-Zip-License.txt`).

**RAR code is not included.** FileZip builds 7-Zip with `DISABLE_RAR_COMPRESS=1`,
so the files under the "unRAR license restriction" are not compiled into the
app, and FileZip can't extract RAR archives.

### LGPL compliance

7-Zip runs as a separate, unmodified executable that FileZip starts as a child
process; FileZip's own code isn't linked with it. You can replace
`Contents/MacOS/7zz` with your own build of 7-Zip. Re-sign the app afterwards
(`codesign --force --deep --sign - FileZip.app`). The exact source code is at
the URL above.
