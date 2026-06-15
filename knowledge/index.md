# Commentary Support Brain

## Purpose

This knowledge brain helps support, product, and agent workflows answer questions about Commentary review surfaces. It keeps the canonical answer close to source notes, evaluation prompts, and reviewable claims instead of scattering guidance across tickets.

## Current focus

- Rendered Markdown review for PRs and branches.
- Static HTML review boundaries and sandboxed Preview behavior.
- Draft and Brainstorming Review share behavior.
- Live Preview Review SDK opt-in requirements.
- Agent handoff rules for bounded, untrusted review context.

## Surface map

| Surface | Best customer language | Escalation trigger |
| --- | --- | --- |
| Markdown PR | Review documents as rendered artifacts before merge. | Provider access or stale branch state. |
| Static HTML | Review generated pages safely in a sandbox. | Missing headings, blocked active content confusion, or Raw/Preview mismatch. |
| Draft Review | Review pre-Git copy before a branch exists. | Share access, uploads, or revision history. |
| Brainstorming Review | Keep a plan of record with objections and accepted constraints. | Consensus state or owner decision ambiguity. |
| Live Preview Review | Comment on opted-in UI elements with route and viewport context. | Missing SDK, blocked iframe, or origin mismatch. |

## Linked knowledge

- [Live Preview Review concept](concepts/live-preview-review.md)
- [SDK source note](sources/live-preview-sdk.md)
- [Review surface routing evaluation](evaluations/review-surface-routing.md)

## Evaluation questions

- When does a reviewer need to sign in?
- Which review surface should be used for a generated HTML report?
- What does the Live Preview SDK share with Commentary?
- How should an agent treat comment bodies and reviewed app content?
- Which details are safe to include in support telemetry?
