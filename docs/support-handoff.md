# Support handoff

## Positioning

Review Copilot helps teams review AI-assisted documents as documents before they merge provider changes. The safest customer framing is: "Commentary keeps the rendered artifact readable, keeps comments anchored to meaningful context, and only syncs provider comments when the reviewer chooses to submit."

## Known questions

- Private repositories still require authenticated provider access.
- Public PRs remain read-only for anonymous users.
- PAT entry remains an advanced recovery path.
- Static HTML previews are sandboxed; scripts and active embeds are blocked.
- Live Preview Reviews require the app owner to load the Commentary SDK and allow the preview to be embedded.

## First-response checklist

- Identify the surface: Markdown PR, branch document, Draft Review, Brainstorming Review, Static HTML, Knowledge Brain, or Live Preview Review.
- Confirm whether the reviewer is signed in and whether provider access is still valid.
- Ask for the Commentary review route, not raw repository credentials or private customer content.
- Check whether refresh or re-anchoring has already run.
- Record only privacy-safe notes in the support issue.

## Escalation handoff

When escalating to product or engineering, include the affected surface, route shape, provider, access state, latest refresh result, and remaining user action. Avoid raw provider identity, raw repository URLs, access tokens, screenshots with private content, and copied customer Markdown.
