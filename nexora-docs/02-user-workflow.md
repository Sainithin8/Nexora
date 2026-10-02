# 02 — V1 User Workflow

## Purpose

Describe the end-to-end user journey and the responsibility of each stage.

## Status and scope

- **Status:** Not yet brainstormed
- **Scope:** User-facing V1 workflow
- **Last updated:** 2026-10-01

## Confirmed decisions

- The high-level sequence is: Market → Opportunity Discovery → Research → Watchlist → Trade Proposal → Risk Check → User Approval → Paper Trade → Position Monitoring → Trade Review.
- User approval comes after deterministic risk validation and before paper order execution.
- The user makes the final decision; a failed hard-risk check cannot be overridden by approval.

## Proposed decisions

None recorded yet.

## Open questions

- What user actions and information should be available at each stage?
- How should the workflow handle an opportunity that lacks enough evidence?
- Which monitoring events should bring an item back to the user's attention?

## Workflow

The stage sequence above is confirmed. Detailed entry conditions, user actions, outputs, and exception paths remain open for discussion.

## Later / V2 ideas

None recorded.

## Related documents

- [Product vision and V1 scope](01-product-vision-and-scope.md)
- [V1 features and requirements](03-features-and-requirements.md)
- [Risk and safety rules](05-risk-and-safety.md)

## Change history

- 2026-10-01 — Created initial outline from the confirmed high-level workflow.

