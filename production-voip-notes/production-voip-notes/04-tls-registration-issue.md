# TLS Was Correct, But Phones Still Failed

A PBX migration included enabling TLS for SIP devices.

Everything appeared correct:

- Valid certificate
- TLS enabled
- SIP port listening
- No obvious errors

Yet phones refused to register.

The problem was not the certificate.

The problem was TLS compatibility.

Some older devices supported only legacy TLS versions, while the PBX was configured for newer standards.

The certificate was valid.

The configuration was correct.

The devices simply could not negotiate a compatible TLS session.

Lesson learned:

Successful TLS deployment requires verifying both security and compatibility.

A valid certificate alone does not guarantee successful registrations.
