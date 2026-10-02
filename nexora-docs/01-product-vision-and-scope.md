# 01 — Product Vision and V1 Scope

## Purpose

Define the user, problem, intended value, and boundaries for Nexora V1.

## Status and scope

- **Status:** Active document — documentation and brainstorming
- **Scope:** Product vision and V1 boundaries
- **Last updated:** 2026-10-01

## Confirmed decisions

- Nexora V1 is a personal AI-assisted trading research and paper-trading platform for one user.
- The initial market is U.S. equities, with regular market sessions and premarket research when useful.
- V1 is paper trading only. The user makes the final decision before a new paper trade executes.
- The primary objective is to find potentially useful opportunities and help evaluate them efficiently, not maximize trade count.
- “NO TRADE” is a valid result when research or risk conditions are not met.
- The project is currently in Documentation + Brainstorming. Do not implement the application until explicitly authorized.
- Work through the six planned documents one at a time and distinguish confirmed, proposed, and open decisions.

## Proposed decisions

None recorded yet.

## Open questions

- What should the initial version consider a “promising” or “qualified” opportunity? Define this in the research and trading logic document.
- What data sources and data freshness expectations are acceptable for V1?
- What is the user's preferred initial timeframe and trading style?

## Product vision

Help one user discover promising U.S. stock opportunities, research them, understand their basic portfolio impact, create clear trade proposals, and paper trade them with user approval.

Nexora should help the user make an informed decision. It should not imply that an AI can predict market outcomes with certainty.

## V1 scope

### In scope

- U.S. equities
- Regular market sessions; premarket research when useful
- Broad market discovery followed by a qualified shortlist
- Research and a watchlist workspace
- Structured trade proposals
- Basic portfolio awareness
- Deterministic risk validation
- User approval before paper order execution
- Paper position monitoring and a trade journal

### Out of scope

- Live trading
- Options, futures, forex, crypto, leverage, or high-frequency trading
- Multi-user, enterprise, team, subscription, or SaaS features
- Complex competing discovery engines
- Advanced portfolio optimization
- Fully autonomous trading

## Product principles

1. Nexora researches; the user makes the trading decision.
2. Paper trading only in V1.
3. Trade proposals explain why the opportunity matters and identify risks.
4. Every proposed trade must pass deterministic risk checks.
5. NO TRADE is valid.
6. Prefer simple, explainable, traceable solutions.
7. Quantitative calculations should be deterministic where appropriate.
8. Do not add features merely because they may be useful someday.

## Later / V2 ideas

Reconsider excluded markets or advanced capabilities only after V1 works and the user requests them.

## Related documents

- [Project instructions](PROJECT_INSTRUCTIONS.md)
- [V1 user workflow](02-user-workflow.md)
- [V1 features and requirements](03-features-and-requirements.md)

## Change history

- 2026-10-01 — Created from the user's V1 project instructions. No additional product decisions inferred.

