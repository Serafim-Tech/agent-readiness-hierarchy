# Open Questions, Challenges & Roadmap
### Where the Agent-Readiness Hierarchy is unfinished — and where it's going

This is the framework arguing with itself. Version 1.0 is a **working model, not settled science** — agentic commerce is barely eighteen months old, and the "right" structure for measuring readiness isn't known yet. This page collects the strongest challenges to the framework, our current (tentative) answers, and the roadmap they imply. A model you can argue with is more useful than one pretending to be finished.

> Licensed under CC BY 4.0. Maintained by Serafim Tech Limited · serafimtech.io

---

## A note on our interest

Serafim Tech builds commercial tools in this space, and this framework maps onto problems our products help solve. We've published it openly, under a permissive license, **precisely so it's useful and verifiable independent of our products** — you can apply the entire framework, score your store, and fix every layer without ever touching anything we sell. We think being upfront about this makes the work more trustworthy, not less. Open and neutral aren't the same thing; we'd rather be transparent about the first than pretend the second.

---

## The status of v1.0

It's a structured, reasoned model — **not yet an empirically validated instrument.** We have not published data proving that a high readiness score *causes* better agent conversion. We believe it does, and we're committing to test it openly (see the roadmap). Until then, treat the score as a well-reasoned hypothesis to act on, not a law to trust blindly.

---

## Open questions & challenges

Each row is a real objection — most raised in stress-testing the framework. "Status" is honest about how settled our answer is.

| # | The challenge | Our current stance | Status |
| :---: | --- | --- | --- |
| 1 | **Do the layers really stack in a strict order?** | No — and v1.0 reflects this. Lower layers *weight* the value of higher ones rather than hard-blocking them; a merchant can work several in parallel. "Fix bottom-up" is a prioritization heuristic, not a law. | Resolved for now — may formalize the weighting later |
| 2 | **Is Trust a layer, or an axis running through all of them?** | We split *transaction* trust (delegated auth, returns, dependability — what a merchant acts on, placed at Layer 4) from *category* trust (will people delegate buying to agents at all — a macro precondition no merchant controls). Layer 4 is the first. | **Genuinely open** — Trust may become a cross-cutting dimension in a future version |
| 3 | **Is one hierarchy category-blind?** | The *layers* are meant to be universal; the *targets within them* are not. Luxury optimizes Trust and brand-legible Comprehension; commodities optimize Transactability and Leverage. Trust is also scored per market (see LAYER-CHECKS). | Partially addressed — needs explicit category profiles |
| 4 | **Can "Optimized (3)" be self-assessed?** | Layer-3 is defined relative to competitors ("agents *prefer* you"), which is hard to grade from the inside without a benchmark. | **Open** — likely needs comparative data or tooling to score honestly |
| 5 | **Does the framework survive a shift to agent-to-agent-by-default commerce?** | Today's layers assume an agent reaching a merchant endpoint. If commerce becomes negotiation-heavy between agents, Transactability and Trust may need reshaping. | **Researching** |
| 6 | **Goods only?** | The framework inherited a goods-centric scope from its source material. Services and B2B are not yet addressed. | **Open** |
| 7 | **Should there be a "Layer 0" for platform/protocol presence?** | Presence depends partly on the platform and the protocol layer existing at all — arguably a precondition beneath Layer 1. | **Open** |
| 8 | **Does the pyramid shape borrow authority it hasn't earned?** | Fair caution about frameworks generally. We've tried to claim only what we can defend — this is a useful lens, not the discovered structure of agentic commerce. | Live with it — calibrate claims, don't overstate |

If you think we've got a layer, an order, or a principle wrong, **that's the invitation.** See [CONTRIBUTING.md](CONTRIBUTING.md) — small fixes as a PR, structural challenges as an issue so we can discuss them first. The canonical version improves through challenge.

---

## Roadmap

Honest and versioned. No promises we can't keep.

### Shipped — v1.0
- The five-layer hierarchy (Presence → Comprehension → Transactability → Trust → Leverage)
- The 0–3 maturity scale
- The two governing principles
- Objective per-layer pass/fail checks · a fillable scorecard · a worked example

### Planned — v1.1
- **Empirical validation.** As agentic traffic grows, publish whether readiness scores actually predict agent-driven conversion — and revise the framework where the data disagrees with the theory. *(This is the most important item; it's what moves v1.0 from hypothesis toward instrument.)*
- Refine the per-layer rubric in [LAYER-CHECKS.md](LAYER-CHECKS.md) as real-world scoring exposes ambiguity
- Re-introduce a clear "merchant-controlled vs. ecosystem-dependent" annotation per layer

### Exploring — v2 territory
- A possible **Trust-as-axis** model (question 2)
- **Category profiles** — what good looks like per layer for luxury vs. commodity vs. services (questions 3, 6)
- How the layers adapt to **agent-to-agent** commerce (question 5)
- A **B2B / services** extension of the goods-centric core (question 6)
- The **"Layer 0"** precondition question (question 7)
- Whether qualitative weighting can become a defensible quantitative model (question 1)

### Out of scope — what this framework will *not* try to be
- We won't build identity, Know-Your-Agent, or payment rails — that's the domain of payment networks and platforms. The framework measures a merchant's *use* of those rails, it doesn't replace them.
- We won't try to resolve *category-level* consumer trust (whether people will delegate buying to agents at all). That's shaped by culture, law, and time — not by any single merchant's diagnostic.

---

## How to weigh in

- **Disagree with an answer above?** Open an issue — tag it `challenge`.
- **Have a worked example, a translation, or a fix?** Open a pull request.
- **Want to argue for a structural change** (a new layer, a re-ordering, Trust-as-axis)? Start an issue so we can discuss before it's merged.

This roadmap is itself open to challenge. If the most important thing isn't on it, tell us.

---

*© 2026 Serafim Tech Limited. Released under CC BY 4.0 — free to use, adapt, and share with attribution.*
