# 05 — Risk and Safety Rules

## Purpose

Define deterministic limits and safety behavior for paper-trade proposals and execution.

## Status and scope

- **Status:** Not yet brainstormed
- **Scope:** Risk validation, user approval, and paper-trading safety
- **Last updated:** 2026-10-01

## Confirmed decisions

- Risk controls are deterministic. AI recommendations cannot override hard rules.
- Every proposed trade must pass risk checks.
- The flow is **Nexora proposes → Risk system validates → User approves → Paper order executes**.
- User approval cannot override a failed hard-risk check.
- Exact risk limits will be decided separately.
- Live trading is outside V1 scope.

## Proposed decisions

None recorded yet.

## Open questions

- What exact limits should apply to position size, exposure, daily loss, single-trade risk, and open positions?
- How should allowed symbols, trading sessions, and a kill switch behave?
- What should happen when required portfolio or market data is unavailable or stale?
- What audit record should be retained for checks, approvals, and paper orders?

## Risk controls

Potential control categories confirmed for future consideration: position-size limits, exposure limits, daily-loss limits, single-trade risk limits, maximum open positions, allowed symbols, trading-session rules, and a kill switch. Values and enforcement details remain open.

## Later / V2 ideas

Live trading is outside V1 and should not be designed into V1 execution flows.

## Related documents

- [V1 user workflow](02-user-workflow.md)
- [Research and trading logic](04-research-and-trading-logic.md)
- [V1 architecture and build plan](06-architecture-and-build-plan.md)

## Change history

- 2026-10-01 — Created initial outline from confirmed project instructions; no thresholds inferred.

