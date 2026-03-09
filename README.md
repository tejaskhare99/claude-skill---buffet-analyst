# Buffett-Style Equity Analyst — Claude Skill

A rigorous, capital-preservation-focused equity analysis skill for Claude. Built on Buffett/Munger principles: durable moats, margin of safety, and normalized earning power — not momentum, not narratives, not vibes.

---------------------------------
### DISCLAIMER
**NOT A FINANCIAL ADVICE, PLEASE DO YOUR OWN RESEARCH AS WELL. THIS TOOL IS FOR RESEARCH PURPOSES ONLY**
---------------------------------

## What It Does

This skill turns Claude into a disciplined equity analyst that:

- **Demands your portfolio context** before any analysis (holdings, cost basis, account types, cash available)
- **Runs 5 hard quantitative gates** — owner earnings yield, ROIC, FCF conversion, leverage, gross margin stability
- **Verifies moats with evidence** — not adjectives, but named mechanisms (patents, switching costs, network effects)
- **Reads the bear case first** — searches for short seller reports and constructs structural bear arguments before any bull thesis
- **Reverse-engineers the price** — solves for what growth the market is *already pricing in*, rather than building a DCF to justify the current price
- **Scores and sizes positions** — weighted scoring framework with Half-Kelly position sizing, capped at 15% per position
- **Refuses to flatter you** — anti-sycophancy rules prevent the AI from softening SELL calls or praising your existing positions

## When It Triggers

Any investing-related question: stock evaluations, portfolio reviews, watchlist checks, "should I buy X?", sector scans, earnings reactions, position sizing, capital deployment — if you mention a ticker or an investment decision, this skill activates.

## Installation

Download `buffett-analyst.skill` from the [Releases](../../releases) page and install it in Claude.

Or copy the `buffett-analyst/` folder into your Claude skills directory.

## Quick Start

Just ask Claude an investing question. The skill will:

1. Ask for your portfolio if you haven't provided it
2. Web-search for live financial data
3. Run the full analytical framework (or a concise version for quick asks)
4. Give you a scored BUY / HOLD / SELL recommendation with the Sleep Test verdict

**Example prompts:**
- "What do you think of COST at these levels?"
- "Run a full deep dive on MSFT"
- "I have $10K to deploy — compare GOOG vs AMZN vs META for me"
- "Review my portfolio and flag any positions I should trim"

## The Framework

| Phase | What It Does |
|---|---|
| **Step 0** | Mandatory portfolio intake — won't proceed without it |
| **Phase 1** | 5 quantitative gates (pass/fail) — filters out capital destroyers |
| **Phase 2** | Moat verification — 5 evidence-based questions |
| **Phase 3** | Bear case first — short thesis before bull thesis |
| **Phase 4** | Reverse DCF — what growth is the price already assuming? |
| **Phase 5** | Signal layers — estimate revisions, insider buying, ROIC acceleration |
| **Scoring** | Weighted action score → BUY (≥1.75) / HOLD / SELL (≤−1.75) |
| **Sleep Test** | "Would I hold this for 10 years with no exit?" — final override |

## License
Please review the license if you are using if for commercial purposes or any other official research purposes.
