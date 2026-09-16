# Yijian Continuity — Technical Public Beta

**Status:** Public distribution channel initialized. **No public binary release has been published yet.**

Yijian Continuity is being built to help people bring an existing AI partner into a portable, reviewable continuity state instead of starting from zero whenever a model, platform, device, or runtime changes.

## What the Technical Beta is designed to do

Yijian Continuity is intended to help you:

1. bring in evidence from an existing AI partner;
2. review what should become lasting Partner state;
3. export a portable Partner Bundle;
4. restore that Partner in another supported context;
5. verify what was preserved, degraded, missing, or still unknown.

## Supported intake paths in the current candidate

- ChatGPT official export / `conversations.json`;
- generic TXT / Markdown transcripts;
- Bridge Snapshot JSON;
- existing Yijian Partner Bundles.

Source AI output is treated as **evidence, not automatic truth**. Protected permissions, cancellations, and `UNKNOWN` / `UNAVAILABLE` states are not silently inferred into canonical Partner state.

## Important Beta limitations

- Windows Technical Beta only.
- The first direct-download build may not yet have broad Windows publisher reputation/signing.
- Partner Bundles and local Partner data are not application-layer encrypted in the current Beta candidate.
- No cloud sync and no remote product telemetry by default.
- Deleting a local Partner does not delete copies already exported or supplied to third-party AI providers.
- Technical verification does not equal Reality PASS or a human continuity verdict.

## Official downloads

When a Technical Beta release is published, download it **only from this repository's Releases page**.

Each binary release must publish `SHA256SUMS.txt`. Verify the downloaded ZIP against the published SHA-256 when practical.

Until a release appears here, there is **no official public Yijian Continuity binary download**.

## Privacy

Yijian Continuity is local-first. Raw imported history is parsed locally and is not persisted merely because it was imported by default.

Do not upload your private Partner Bundle, full chat history, API credentials, recovery codes, or local personal paths in a public bug report.

See `PRIVACY.md`, `SECURITY.md`, and `SUPPORT.md` before using a future Beta release.

## Technical Beta feedback

The most important result is not download count. It is whether a previously existing AI partner can be restored in a way that the user recognizes as meaningfully continuous.

When reporting a problem, include only non-sensitive details such as:

- software version;
- Windows version;
- intake type;
- standardized error code;
- which step failed: launch / intake / review / export / restore / verify.

## Ownership

Your Partner state belongs to you. Software updates must not silently expand permissions, revive cancelled tasks, fabricate unknown facts, or rewrite the Partner relationship merely because the application version changed.

## Repository boundary

This repository is the **public distribution and feedback channel**. It is intentionally separate from private development, continuity governance, internal experiments, and protected state. Public distribution does not imply publication of private development history or user Partner data.
