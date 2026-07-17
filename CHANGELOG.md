## 0.1.1

- Rename the example file to match the package name so pub.dev picks it
  up.

## 0.1.0

Initial release, vendoring simdjson 4.6.4.

- `SimdJsonDocument`: parse once, materialize only the subtrees you
  read, addressed by RFC 6901 JSON Pointers. 5-15x faster than full
  decoding when reading selected fields from large documents.
- `simdJsonDecodeBytes` / `simdJsonDecode`: whole-document decoding
  with the same result shapes as `jsonDecode`.
- Native code builds automatically via Dart build hooks (Dart 3.10+);
  no manual native setup.
