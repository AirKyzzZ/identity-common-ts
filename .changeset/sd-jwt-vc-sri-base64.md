---
'@sd-jwt/sd-jwt-vc': patch
---

Fix the `vct#integrity` and `extends#integrity` checks: the digest is now compared as base64, as defined by W3C Subresource Integrity, instead of hex. When the integrity metadata lists several hashes, only the strongest supported algorithm (`sha256`, `sha384`, `sha512`) is checked and any of its values may match. Integrity metadata without a supported algorithm is rejected.
