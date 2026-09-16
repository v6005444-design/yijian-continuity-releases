# Security — Yijian Continuity Technical Public Beta

**Status:** Public distribution channel initialized. No public binary release has been published yet.

## Sensitive vulnerability reports

Do **not** post credentials, private Partner Bundles, full chat exports, relationship/memory content, exploit details, or local personal paths in a public issue.

Before the first public binary release, this repository must have an explicit private vulnerability-reporting channel enabled. Until that channel is confirmed, use public issues only for non-sensitive security questions or to request a private contact path without disclosing vulnerability details.

## Safe initial report fields

For non-sensitive reports, include only:

- release version;
- Windows version;
- affected step;
- standardized error code;
- whether the issue involves intake, local API, Bundle parsing, restore, update, or verification.

If diagnosis requires sensitive evidence, stop and establish an explicit redaction/consent path first.

## Current security boundary

The Technical Beta candidate is local-first and uses a loopback-only local service. Current release hardening includes session authorization, Host/Origin/cross-site checks, bounded request/Bundle sizes, malicious ZIP resource controls, a single-instance launcher, and explicit local-process exit.

Current limitations include:

- Partner Bundle confidentiality/encryption is not yet implemented;
- local Partner data is not application-layer encrypted at rest;
- no independent external penetration test has been completed;
- direct Windows distribution may not yet have broad publisher reputation/signing;
- local deletion is local-copy-only and cannot revoke copies already exported or given to third parties.

## Official release authenticity

Official releases must be distributed only through this designated Yijian release repository and accompanied by SHA-256 checksums. Wider consumer distribution should use Microsoft Store/MSIX or a stable trusted code-signing identity.

A checksum is useful only when obtained from the official release channel; it does not make arbitrary third-party repackaging official.
