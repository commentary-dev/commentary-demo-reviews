# Review Copilot Launch Narrative

## The problem

AI-generated documents are being reviewed as raw diffs even when the decision depends on reading flow, accuracy, stakeholder language, and whether the final artifact makes sense outside a code review.

Reviewers lose time reconstructing context from source lines. Agents receive incomplete comments. Support inherits launch copy that nobody read like a customer would.

## The product answer

Commentary opens the rendered document first, keeps source tools nearby, and anchors comments to meaningful review context. The review workspace treats provider comments as synchronized representations, not as the only place collaboration can happen.

## What this launch demonstrates

- Rendered Markdown review for PRs and branches.
- Static HTML review for generated reports.
- Draft and Brainstorming Reviews for app-native workflows before or beside Git.
- Live Preview Reviews for selected UI elements in opted-in browser previews.
- Agent handoff through bounded, untrusted review context.

## Launch risks

| Risk | Mitigation |
| --- | --- |
| Customers expect arbitrary website inspection | Explain SDK opt-in and host frame requirements. |
| Support cannot explain static HTML sandboxing | Ship the FAQ before expanding the preview. |
| Demo samples feel too synthetic | Use representative Markdown, HTML, decks, and app routes. |

## The launch ask

Approve a controlled rollout for documentation-heavy teams with support coverage, rollback ownership, and validated public demos in place.

## Decision

Launch after the support FAQ, customer memo, migration report, Live Preview sample, and resettable review records pass review.
