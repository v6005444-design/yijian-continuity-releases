# Yijian Continuity — Technical Public Beta

**Status:** Technical Public Beta is now available for Windows. This is a **pre-release**, not a Stable release.

**Official release:** https://github.com/v6005444-design/yijian-continuity-releases/releases/tag/v0.1.0-beta

Yijian Continuity is being built for people who already have an AI assistant, collaborator, teacher, creative partner, or companion they do not want to lose whenever a model, platform, device, or runtime changes.

The goal is not to copy every old chat forever. The goal is to help a user bring forward the important identity, relationship, preferences, permissions, cancellations, provenance, and unresolved unknowns that make a long-running AI relationship or workflow recognizable and usable.

## Pilot 1 — we are looking for the first real testers

We are currently recruiting a **small first cohort (3–5 people)** for a Stranger Partner Recovery Test.

You may be a good fit if:

- you have used ChatGPT, Claude, Gemini, Character.AI, Replika, or another AI system over time;
- the AI has accumulated meaningful context, working style, preferences, project history, or relationship context;
- losing that continuity because of a model/platform change would matter to you;
- you use Windows and are comfortable trying an early Technical Beta;
- you are willing to tell us plainly whether the restored result feels meaningfully continuous, partly continuous, or not continuous.

You do **not** need to think of your AI as a human-like companion. Long-term work, learning, research, creative, coaching, and personal-assistant relationships are also relevant.

### What testers do

1. Download the official Technical Beta release.
2. Bring evidence from an existing AI partner/workflow into Yijian Continuity.
3. Review what should and should not become lasting Partner state.
4. Export and restore the Partner state.
5. Tell us what was preserved, degraded, missing, or wrong.
6. Give your own human continuity judgment.

The most important question is not “Did the software run?” It is:

> **After restore, do you recognize this as meaningfully continuous with the AI partner or long-running AI relationship you had before?**

If you want to participate, see the open Pilot 1 recruitment issue in this repository. Please do not post private chat history or Partner Bundles publicly.

## What the Technical Beta is designed to do

Yijian Continuity is intended to help you:

1. bring in evidence from an existing AI partner;
2. review what should become lasting Partner state;
3. export a portable Partner Bundle;
4. restore that Partner in another supported context;
5. verify what was preserved, degraded, missing, or still unknown.

## Supported intake paths in the current Beta

- ChatGPT official export / `conversations.json`;
- generic TXT / Markdown transcripts;
- Bridge Snapshot JSON;
- existing Yijian Partner Bundles.

Source AI output is treated as **evidence, not automatic truth**. Protected permissions, cancellations, and `UNKNOWN` / `UNAVAILABLE` states are not silently inferred into canonical Partner state.

## Important Beta limitations

- Windows Technical Beta only.
- The direct-download build may not yet have broad Windows publisher reputation/signing.
- Partner Bundles and local Partner data are not application-layer encrypted in the current Beta candidate.
- No cloud sync and no remote product telemetry by default.
- Deleting a local Partner does not delete copies already exported or supplied to third-party AI providers.
- Technical verification does not equal Reality PASS or a human continuity verdict.

## Official downloads and verification

Download Yijian Continuity **only from this repository's Releases page**.

The current release publishes `SHA256SUMS.txt`. Verify the downloaded ZIP against the published SHA-256 when practical.

## Privacy

Yijian Continuity is local-first. Raw imported history is parsed locally and is not persisted merely because it was imported by default.

Do not upload your private Partner Bundle, full chat history, API credentials, recovery codes, or local personal paths in a public bug report.

See `PRIVACY.md`, `SECURITY.md`, and `SUPPORT.md` before using the Beta.

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
