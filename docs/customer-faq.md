# Customer FAQ

## What changes for reviewers?

Reviewers start in the rendered document, comment on sections or selected text, and use Raw or Diff only when source detail matters. The goal is to review the artifact the way customers and teammates will read it, without losing Git-backed traceability.

## Does GitHub remain the source of truth?

Yes. Commentary keeps the repository and provider permissions authoritative. App-native review threads are the primary working record, and provider comments are synchronized representations when a reviewer submits feedback.

## What can anonymous users do?

Public PRs can be opened read-only without sign-in. Commenting, replies, refreshes that need private credentials, private repositories, and review submission require authentication through OAuth or the advanced PAT recovery path.

## Which surfaces are in this preview?

| Surface | Use when | Review benefit |
| --- | --- | --- |
| Markdown PR | Docs, release notes, FAQs, runbooks | Rendered prose and source context stay together. |
| Static HTML | Generated reports or exported pages | The page is readable while active content stays sandboxed. |
| Draft Review | Pre-Git memos or customer copy | Teams can comment before creating a branch. |
| Brainstorming Review | Plans that need consensus | Objections, accepted constraints, and owner decisions stay visible. |
| Live Preview Review | Interactive frontend previews | Comments attach to selected UI elements with route and viewport context. |

## Who should use the preview first?

Teams reviewing generated launch docs, release notes, support playbooks, Markdown-heavy product pages, and static reports that currently get reviewed as raw diffs.

## What should support say if a customer asks about AI?

Commentary does not ask customers to trust an agent blindly. It gives agents scoped review context, keeps human comments first-class, and leaves provider access control in place.
