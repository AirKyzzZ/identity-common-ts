---
'@owf/cose': minor
'@owf/crypto': minor
'@owf/eudi-access-certificate': minor
'@owf/eudi-attestation-schema': minor
'@owf/eudi-jades': minor
'@owf/eudi-lote': minor
'@owf/eudi-registration-certificate': minor
'@owf/eudi-sca': minor
'@owf/eudi-tl': minor
'@owf/identity-common': minor
'@sd-jwt/core': minor
'@sd-jwt/sd-jwt-vc': minor
'@owf/token-status-list': minor
'@owf/x509': minor
---

Drop the CommonJS build from all packages; only ESM is now published. All environments targeted by this library support ESM natively. This removes the dual-package hazard that caused `instanceof` checks to fail in Metro/Hermes and similar single-module-system runtimes.
