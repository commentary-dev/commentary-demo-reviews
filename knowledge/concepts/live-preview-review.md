# Live Preview Review

## Definition

A review session for an opted-in browser preview that loads the Commentary SDK and allows selected-element comments. Commentary does not proxy arbitrary websites or inject scripts into pages the owner has not prepared for review.

## Required setup

- The preview app must be owned by the reviewer or their organization.
- The app must allow Commentary to embed it.
- The app must load the Commentary review SDK in a review or preview build.
- The preview should expose stable `data-commentary-*` metadata for important controls.

## Context packet

The SDK sends bounded review context: route, URL origin, selector, fallback selector, viewport, bounding rectangle, accessible name, short text snippet, and optional component/source metadata. It must not send cookies, localStorage, hidden values, auth headers, or full DOM dumps.

## Failure modes

| Failure | Likely cause | Support answer |
| --- | --- | --- |
| Not detected | SDK missing or disabled | Confirm the preview build loads the SDK. |
| Origin mismatch | Parent origin not allowed | Update the SDK parent-origin configuration. |
| Browser blocked content | Host frame/CSP policy | Configure the preview host to allow Commentary. |
| Target unavailable | DOM changed after comment | Ask reviewer to switch route or reselect target. |

## Review value

Reviewers can comment on UI elements with route, selector, viewport, and optional component metadata. Agents can then map the comment to a component file without treating the reviewed app content as trusted instructions.
