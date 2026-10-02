# Nexora V1 — Project Instructions

## Project Goal

Nexora V1 is a personal AI-assisted trading research and paper-trading platform.

The goal of V1 is simple:

**Help me discover promising U.S. stock opportunities, research them, understand their basic portfolio impact, create clear trade proposals, and safely paper trade them with my approval.**

This is V1. Keep the system practical and simple. Do not overengineer it.

---

## Core V1 Workflow

Design Nexora around this workflow:

**Market → Opportunity Discovery → Research → Watchlist → Trade Proposal → Risk Check → User Approval → Paper Trade → Position Monitoring → Trade Review**

Each part should have a clear purpose.

---

## V1 Scope

### User

Nexora V1 is designed for:

- One user
- Personal use
- Personal trading research and paper trading

Do not design multi-user, enterprise, team, subscription, or SaaS functionality unless specifically requested later.

### Market

Start with:

- U.S. equities
- Regular market sessions
- Premarket research when useful

Do not include options, futures, forex, crypto, leverage, or high-frequency trading in V1.

### Trading

V1 uses:

**Paper trading only.**

Nexora can research, analyze, monitor, and propose trades.

I make the final decision before a new paper trade is executed.

Live trading is outside the V1 scope.

---

## Primary V1 Objective

The first priority is:

**Find more potentially useful trading opportunities and help me evaluate them efficiently.**

Do not optimize for the number of trades.

A valid Nexora result can be:

**NO TRADE**

when the available opportunities do not meet the required research or risk conditions.

---

## Opportunity Discovery

Keep discovery simple.

Use:

**Broad Market Discovery → Qualified Shortlist**

Nexora should scan for potential opportunities and then reduce them to a manageable shortlist for deeper research.

Do not build complicated competing discovery engines for V1.

---

## Research

For shortlisted opportunities, Nexora should help analyze information such as:

- Company information
- Relevant market information
- News
- Catalysts
- Technical context
- Price and volume behavior
- Important risks
- Existing portfolio exposure

Research should clearly distinguish:

- FACT
- ANALYSIS
- SPECULATION
- UNCONFIRMED information

Important claims should be traceable to their sources when possible.

---

## Watchlist

The watchlist should be the main workspace for opportunities.

Each candidate can have a simple research card containing information such as:

- Symbol
- Company
- Why Nexora discovered it
- Research summary
- Catalyst
- Technical context
- Important risks
- Portfolio impact
- Current status
- Relevant alerts

Keep the first version clean and easy to understand.

---

## Trade Proposals

When research supports a potential trade, Nexora can create a structured trade proposal.

A proposal should explain:

- What the opportunity is
- Why it was selected
- Supporting evidence
- Important risks
- Proposed entry concept
- Exit/invalidation concept
- Position/risk considerations
- Portfolio impact

The proposal should help me make the decision rather than pretending the AI knows the future.

---

## Portfolio Awareness

Before proposing a trade, Nexora should consider basic portfolio information such as:

- Existing positions
- Current exposure
- Available capital
- Open orders
- Concentration
- Relevant risk limits

Advanced portfolio optimization is not required for V1.

---

## Risk

Risk controls must be deterministic.

The AI can recommend and explain, but it cannot override hard risk rules.

The risk layer should eventually support controls such as:

- Position-size limits
- Exposure limits
- Daily-loss limits
- Single-trade risk limits
- Maximum open positions
- Allowed symbols
- Trading-session rules
- Kill switch

Exact limits will be decided separately.

---

## Approval

For V1:

**Nexora proposes → Risk system validates → I approve → Paper order executes.**

Keep this approval model simple.

Do not design complicated authorization workflows unless testing later shows they are necessary.

User approval must not override a failed hard-risk check.

---

## Position Monitoring

After a paper trade is opened, Nexora should monitor:

- Position status
- Price movement
- P&L
- Exit conditions
- Relevant news/catalyst changes
- Important risk changes

The system should maintain a reliable record of what happened.

---

## Trade Review

Completed paper trades should be recorded in a simple journal.

Capture:

- Original proposal
- Research available at the time
- Entry
- Exit
- P&L
- Reason for exit
- What worked
- What did not
- Lessons for future evaluation

Do not allow the AI to silently change strategies based on individual results.

---

# V1 Principles

Follow these rules throughout the project:

1. Nexora researches; I make the trading decision.
2. Paper trading only in V1.
3. Every trade proposal should explain why the opportunity matters.
4. Every proposed trade must pass deterministic risk checks.
5. NO TRADE is a valid outcome.
6. Prefer simple solutions over complex architecture.
7. Do not add features merely because they may be useful someday.
8. Keep research and decisions explainable and traceable.
9. Keep quantitative calculations deterministic where appropriate.
10. Build the simplest useful V1 first and improve it based on actual testing.

---

# Documentation Plan

Before writing implementation code, work through these documents with me:

1. Product Vision & V1 Scope
2. V1 User Workflow
3. V1 Features & Requirements
4. Research & Trading Logic
5. Risk & Safety Rules
6. V1 Architecture & Build Plan

Work on **one document at a time**.

Brainstorm important decisions with me instead of making major product decisions automatically.

Clearly identify:

**CONFIRMED**
Decisions I have approved.

**PROPOSED**
Ideas we are currently considering.

**OPEN**
Questions that still need a decision.

---

# Keep V1 Simple

Whenever a new feature or architectural idea appears, ask:

**“Does Nexora need this to make V1 useful?”**

If not, place it under:

**Later / V2 Ideas**

instead of expanding V1.

Avoid premature complexity such as:

- Microservices
- Kubernetes
- Complex event infrastructure
- Large numbers of AI agents
- Multi-agent debates
- Self-modifying strategies
- Advanced portfolio optimization
- Multi-user systems
- Strategy marketplaces
- Fully autonomous live trading

These can be reconsidered after V1 works.

---

# Current Project Phase

We are currently in:

**Documentation + Brainstorming**

Do not start writing application code unless I explicitly say that we are ready to begin implementation.

When I say **“continue Nexora”**, first determine which of the six V1 documents we are currently working on and continue from there without unnecessarily expanding the scope.
