# Privacy — Yijian Continuity Technical Public Beta

**Status:** Public distribution channel initialized. No public binary release has been published yet.

This notice describes the intended behavior of the current Windows Technical Public Beta candidate. Material privacy changes should be disclosed before activation rather than silently assumed.

## Local-first storage

By default, Partner data is stored under the current user's home directory in `.yijian/partners`, unless the user explicitly configures another `YIJIAN_DATA_DIR` location.

The application exposes the active data directory in its Privacy & Data view.

**Current local Partner files are not encrypted by Yijian Continuity at the application layer.** Local-first means the application does not require those files to be uploaded to our cloud; it does not mean they are automatically encrypted at rest. Confidentiality also depends on operating-system account permissions, device/full-disk encryption, and the security of the user's machine.

## Existing-Partner Intake

The current candidate can locally parse supported ChatGPT export ZIP/JSON files and UTF-8 role-marked text/Markdown transcripts, review a provider-neutral Bridge Snapshot, or restore an existing Yijian Partner Bundle.

Imported sources may contain highly sensitive personal conversation history. In the current candidate:

- the selected source file is read by the local application process;
- the source is not automatically uploaded to a Yijian cloud service;
- raw imported chat history is **not copied into the Partner database by default**;
- the intake pipeline persists user-confirmed Partner state plus provenance such as source evidence SHA-256 and available message/time references;
- direct adapters do not automatically infer permissions, cancellations, or `UNKNOWN` / `UNAVAILABLE` state from raw history;
- memory candidates remain uncommitted until the user explicitly selects them.

Users should keep original provider exports under their own control. Deleting an imported Partner does not delete the original export file.

The current direct-intake file limit is 32 MiB. This is an implementation and safety boundary, not a promise that all provider exports fit within it.

## Local web service

The bundled application binds only to a loopback address. The release launcher chooses a random local port and creates a random local-session token for each running instance. API requests require that token and apply local Host/Origin/cross-site checks.

The token reduces the risk that an unrelated web page can call the local API. It is not a substitute for operating-system account security and does not protect against malicious software already running with the same user's privileges.

## Network behavior

The current candidate does not include an account system, cloud synchronization, remote telemetry, analytics collection, or an embedded AI-provider API-key workflow.

If a future version adds external network services, cloud sync, auto-update, remote metrics, or provider connectors, those capabilities require separate disclosure and testing before activation.

## Exported Partner Bundles

Exported Partner Bundles may contain partner identity, relationship instructions, selected memories, protected state, and continuity/provenance information.

**Current Public Beta Bundles are not encrypted.** Integrity bindings can detect certain modifications but do not provide confidentiality. Treat an exported Bundle like a sensitive personal backup.

The application does not automatically upload exported Bundles.

## Deletion

The current candidate can delete a selected local Partner directory only after explicit user confirmation. This deletes the local application copy on that machine.

Deleting the local copy does **not** automatically:

- delete the original provider export chosen for intake;
- delete exported Partner Bundles;
- erase copies stored on another device;
- revoke a Bundle already shared with another runtime/provider;
- prove cryptographic erasure of external copies.

Portable revocation/deletion propagation is a future capability and must not be inferred from a local delete action.

## Third-party AI providers

The application can generate manual handoff packages for another AI runtime/provider. It does not automatically transmit those packages. Once a user intentionally supplies data to an external AI service, that service's own privacy and retention practices apply. Yijian Continuity cannot claim control over an external provider's copies.

## Diagnostics and metrics

The app can generate a sanitized diagnostics JSON intended for support. The current diagnostics contract excludes Partner content, Partner IDs, and local filesystem paths.

Current remote telemetry remains **off**. Download counts, voluntary issue reports, and explicit pilot feedback must not be confused with successful restores or active users.

## Current limitations

This is a Technical Public Beta candidate, not a completed privacy or security certification. No claim is made that the software has passed an independent security audit, formal privacy certification, Microsoft Store certification, or production-scale external penetration testing.
