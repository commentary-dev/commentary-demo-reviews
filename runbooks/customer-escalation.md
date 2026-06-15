# Customer escalation runbook

## When to use this runbook

Use this path when a customer reports that review comments are missing, attached to stale content, blocked by provider access, or disconnected from the document they expected to review.

## First response

Confirm whether the customer is reviewing a public PR, a private PR, a branch document, a Draft Review, a Brainstorming Review, a Static HTML report, a Knowledge Brain, or a Live Preview Review. Ask for the Commentary route and the visible error state. Do not ask for raw access tokens, raw private repository URLs, screenshots with customer content, or copied private Markdown.

## Triage checklist

- Check whether the user is signed in.
- Check whether the repository provider still grants read access.
- Check whether the review is public read-only or requires authenticated writes.
- Check whether refresh or re-anchoring has already run.
- For Live Preview Reviews, verify that the preview app is frameable and the SDK status is Connected.
- Capture the review route without copying raw customer repository URLs into telemetry.

## Decision table

| Symptom | Likely cause | First action |
| --- | --- | --- |
| Comment button is unavailable | Anonymous or read-only viewer | Ask the reviewer to sign in with OAuth. |
| File list is stale | Branch or PR changed after first load | Run refresh and confirm the new head state. |
| Comment moved to unresolved | Anchor text changed or disappeared | Use re-anchor state and inspect nearby semantic blocks. |
| Live preview is blank or blocked | Host frame/CSP settings or missing SDK | Open the preview directly, then check SDK and frame guidance. |
| Static HTML interaction does nothing | Sandbox blocks scripts | Explain that HTML Review is for safe static review, not live app behavior. |

## Resolution handoff

Summarize the affected review surface, the access state, the latest refresh result, the user-visible failure state, and the remaining user action. If escalation is needed, include only privacy-safe identifiers and the Commentary route.
