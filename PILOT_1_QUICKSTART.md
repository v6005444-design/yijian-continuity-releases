# Pilot 1 Quick Start — First Stranger Continuity Test

This is the shortest supported path for the current Windows Technical Beta.

## Goal

The test is not merely whether Yijian Continuity launches.

The important question is:

> After restore, do you recognize the result as meaningfully continuous with the AI partner or long-running AI workflow you had before?

A negative result is useful. "Partly continuous" and "not continuous" are valid outcomes.

## Before you start

- Windows only for this Technical Beta.
- Download only from the official GitHub Release.
- Do not use a third-party repackaged build.
- Read `PRIVACY.md`, `SECURITY.md`, and `SUPPORT.md`.
- Current Partner Bundles/local Partner data are not application-layer encrypted by Yijian Continuity.
- Do not use public GitHub issues to post private chat history or Partner Bundle contents.

## 5-step test

### 1. Download
Use the official release:
https://github.com/v6005444-design/yijian-continuity-releases/releases/tag/v0.1.0-beta

When practical, verify the ZIP against `SHA256SUMS.txt`.

### 2. Bring Existing Partner
Use one supported input:
- ChatGPT official export / `conversations.json`
- TXT / Markdown transcript
- Bridge Snapshot JSON
- existing Yijian Partner Bundle

### 3. Review
Review the candidate Partner state.

Do not accept something merely because the old AI said it.
Pay special attention to:
- identity / role
- relationship / working style
- permissions
- cancellations
- important memories
- unresolved UNKNOWN / UNAVAILABLE items

### 4. Export -> Restore -> Verify
Export the Partner Bundle, restore it in the supported flow, and run verification.

Record only the high-level outcome:
- technical restore succeeded / partly succeeded / failed
- what was preserved
- what was missing or wrong

### 5. Give your human continuity verdict
Open a new GitHub issue and select:

**Pilot 1 continuity feedback**

Choose one:
- Meaningfully continuous
- Partly continuous
- Not continuous
- Could not reach continuity judgment because the technical flow failed

Also answer whether you would trust this workflow enough to use it again before switching models/platforms.

## Privacy boundary

Do NOT publish:
- full AI/chat exports
- Partner Bundle contents
- partner identity/relationship/memory text
- API keys, passwords, tokens, recovery codes
- local personal file paths
- private information about other people

High-level descriptions are enough.

## What counts as a successful Pilot 1 result?

A useful result is any honest completed outcome, including failure.

Technical success does not automatically mean relationship/identity continuity succeeded.
Human continuity judgment remains a separate reality gate.
