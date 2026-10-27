---
"@openid4vc/openid4vci": patch
---

Add `Openid4vciIssuer.parseCredentialRequestPayload` to parse a Credential Request that was already decrypted, without the transport encryption rules of `parseCredentialRequest`. This allows parsing a decrypted request that contains `credential_response_encryption` again later in the flow.
