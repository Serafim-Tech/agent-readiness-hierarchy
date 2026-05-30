# The Agent-Readiness Hierarchy™
### An open framework for agentic-commerce readiness

**Maintained by Serafim Tech Limited** · serafimtech.io
Version 1.0 · 2026 · Licensed under Creative Commons Attribution 4.0 (CC BY 4.0)

*Serafim Tech Limited · Company No. 12884078 · Registered in England & Wales*

---

> **Open framework.** This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/). You are free to **share** and **adapt** it for any purpose, including commercially — provided you give appropriate credit to Serafim Tech, link to the license, and indicate if changes were made. We encourage merchants, platforms, agencies, and tool-builders to use it, teach it, and build on it.

---

## What this is

The Agent-Readiness Hierarchy is a simple, reusable model for answering one question: **how ready is a store for AI agents that shop on a customer's behalf?**

As commerce shifts from humans browsing pages to agents acting on intent, "are we ready?" became a question every merchant needs to answer and almost none could measure. This framework turns that vague question into a diagnostic — a way to locate any store on a map, score it, and know exactly what to fix next, in priority order.

It is deliberately open. A shared, free vocabulary for agent-readiness is more useful to everyone — including us — than a proprietary one locked in a drawer.

---

## The core idea

An AI agent acting for a shopper engages with five things, and lower layers **weight** the value of higher ones: a brilliant promotion an agent can't parse (Layer 5 on a weak Layer 2) isn't worth zero, but it's worth far less than it should be. The layers don't strictly *block* each other — a merchant can work several in parallel — but effort spent high in the stack pays off only as far as the layers beneath it support it. So the hierarchy is generally read — and prioritized — **from the bottom up**.

```
                  ┌─────────────────────────┐
                  │   5 · LEVERAGE          │   Can I capture value & learn?
                ┌─┴─────────────────────────┴─┐
                │     4 · TRUST               │   Can the transaction be trusted?
              ┌─┴─────────────────────────────┴─┐
              │       3 · TRANSACTABILITY       │   Can an agent actually buy?
            ┌─┴─────────────────────────────────┴─┐
            │         2 · COMPREHENSION           │   Can it understand what I sell?
          ┌─┴─────────────────────────────────────┴─┐
          │           1 · PRESENCE                  │   Can an agent find & reach me?
          └─────────────────────────────────────────┘
                          build up ↑
```

| Layer | The question the agent is asking | What lives here | Mostly in your control? |
|---|---|---|---|
| **5 · Leverage** | Can I (the merchant) capture value and learn? | Agent-readable promotions, loyalty & bundles; agent attribution & observability; new monetization; the data feedback loop | Yes |
| **4 · Trust** | Can the transaction be trusted? | Delegated authorization, Know-Your-Agent posture, transparent returns & substitution, dependability signals | Partly — shared with payment networks, identity standards & regulators |
| **3 · Transactability** | Can an agent actually buy? | Cart accepts agent line items, computes totals, returns a working checkout URL; payment handlers; fulfillment options | Mostly |
| **2 · Comprehension** | Can it understand what I sell? | Catalog quality, structured data, variant resolution, semantic metadata, localization | Yes |
| **1 · Presence** | Can an agent find and reach me at all? | Discovery profile reachable & parseable; live agent endpoint; agentic channels enabled | Partly — shared with your platform & the protocol layer |

The base is widest on purpose: presence is the broadest foundation that everything else leans on, and each layer narrows because fewer merchants get that far. **Your weakest low layer is usually your real bottleneck** — a brilliant Layer 5 sitting on a broken Layer 1 delivers a fraction of its potential in practice.

---

## The maturity scale

Score **each layer 0–3**. This is what turns the hierarchy from a diagram into a diagnostic. The scoring is still partly judgment-based today; a detailed, checkable rubric for each layer at each score is the priority for the next version (see *Known limitations*).

| Score | State | Meaning |
|---|---|---|
| **0** | Absent | The capability isn't there; agents fail at this layer. |
| **1** | Basic | Present but incomplete or unreliable (e.g. catalog exists but variants don't resolve). |
| **2** | Functional | Works correctly for a competent agent, end to end. |
| **3** | Optimized | Works — *and* is structured so agents prefer you over a comparable merchant. |

**Reading the scores**
- **Bottleneck** = the lowest weak layer at the bottom of the stack. Fix it first, regardless of how good a higher layer looks.
- **Overall readiness** = the highest layer you reach scoring ≥2 with no gaps beneath it. You're only as ready as your first weak floor.
- **Near-term target** for most merchants: 2s across Layers 1–3, then push Layers 2 and 5 toward 3 — comprehension and leverage are where a focused smaller merchant out-competes a bigger, sloppier one.

---

## The two governing principles

These keep the framework strategic, not merely technical. They apply at every layer.

**1 · Agent-ready, not agent-dependent.**
Expose your capabilities to agents while fighting to keep what matters: stay the merchant of record where you can, and protect identity, payment authorization, and the post-purchase relationship and data. The pressure toward disintermediation is real and you may not win every inch of it — but readiness should be a deliberate trade, not a surrender of the customer relationship by default.

**2 · The same machinery serves humans and agents.**
Every layer, done well, also improves the human experience — clean data, a cart that always computes totals, transparent returns, exposed promotions. The work is therefore never wasted, even if agentic adoption arrives slower than predicted. Build for the agent; the human benefits too.

---

## How to use it

1. **Diagnose.** Score all five layers 0–3 — measure, don't guess.
2. **Find the floor.** Identify the lowest weak layer; that's your bottleneck.
3. **Fix bottom-up.** Bring each layer to ≥2 before investing above it.
4. **Optimize selectively.** Push Comprehension (2) and Leverage (5) toward 3 — that's your competitive edge.
5. **Re-score and repeat.** Readiness is a loop, not a one-time project; protocols and agents keep moving.

---

## Status: a working model, not settled science

This is **version 1.0** — a structured, reasoned model, not yet an empirically validated instrument. We have not yet published data proving that a high readiness score *causes* better agent conversion. We believe it does, and we're committing to test it openly: as agentic traffic grows, we'll publish whether readiness scores actually predict agent-driven revenue, and revise the framework where the data disagrees with the theory. Treat the score as a well-reasoned hypothesis to act on, not a law to trust blindly.

**A note on our interest.** Serafim Tech builds commercial tools in this space, and this framework maps onto problems our products help solve. We've published it openly, under a permissive license, precisely so it's useful and verifiable *independent of* our products — you can apply the whole framework without ever touching anything we sell. We think being upfront about this makes the work more trustworthy, not less.

---

## Known limitations & how to challenge this

We publish the framework's weaknesses alongside the framework, because a model you can argue with is more useful than one that pretends to be finished. The strongest objections, and our current responses:

- **"The layers don't really stack in a strict order."** Correct — and v1.0 reflects this: lower layers *weight* the value of higher ones rather than hard-blocking them. A merchant can and often should work several in parallel. The bottom-up ordering is a prioritization heuristic, not a law of nature.
- **"Trust is the foundation of the whole category, so why is it Layer 4?"** Fair tension. We distinguish *transaction-level* trust (delegated authorization, returns, dependability — what a merchant can act on, placed at Layer 4) from *category-level* trust (will consumers delegate purchasing to agents at all — a macro precondition outside any single merchant's control). Reasonable people may redraw this; we'd welcome the argument.
- **"It mixes things merchants control with things they don't."** True, which is why each layer is now annotated for control. Presence and Trust are partly ecosystem- and platform-dependent. The framework tells you where your effort moves the needle versus where you're waiting on others.
- **"The 0–3 scale is subjective."** Currently, yes. A concrete per-layer rubric is the top priority for v1.1. Until then, treat scores as directional.
- **"A single hierarchy is category-blind."** The *layers* are intended to be universal; the *targets within each layer* are not. A luxury brand optimizes Trust and brand-legible Comprehension; a commodity reseller optimizes Transactability and Leverage. High-consideration categories rationally plateau lower on agent-delegation than commodities do.
- **"The layers overlap."** They do. Structured data serves both Comprehension and Transactability; promotions touch both Comprehension and Leverage. Placement reflects the *primary* question a capability answers, not an exclusive home.
- **"A pyramid makes any idea look more rigorous than it is."** A fair caution about frameworks generally. We've tried to claim only what we can defend — this is a useful lens, not the discovered structure of agentic commerce. Hold us to that.

If you think we've got a layer, an order, or a principle wrong, we want to hear it. The canonical version improves through challenge.

---

## Origins & attribution

The Agent-Readiness Hierarchy is an original framework developed by Serafim Tech. It synthesizes and builds on publicly available thinking about agentic commerce, including McKinsey & QuantumBlack's *The Agentic Commerce Opportunity* (October 2025) and Serafim Tech's own diagnostic work. Those sources are cited as intellectual influences; the layered hierarchy, the maturity scale, and the governing principles are Serafim Tech's own contribution, and it is this contribution that is offered here under CC BY 4.0.

---

## How to cite

> Serafim Tech (2026). *The Agent-Readiness Hierarchy: An open framework for agentic-commerce readiness*, v1.0. Licensed under CC BY 4.0. Available at serafimtech.io.

---

## About Serafim Tech

Serafim Tech builds the capability layer for agentic commerce — composable, agent-readable commerce primitives that let merchants be found, understood, and transacted with by AI agents. We publish this framework openly because a shared standard for agent-readiness helps the whole ecosystem mature, merchants and builders alike.

**Serafim Tech Limited**
Registered office: 124–128 City Road, Islington, London, EC1V 2NX, United Kingdom
Company No. 12884078 · VAT 359617656 · Registered in England & Wales
serafimtech.io

*Note: Serafim Tech Limited (agentic commerce, serafimtech.io) is unrelated to any similarly named gaming or hardware brand.*

---

*© 2026 Serafim Tech Limited (Company No. 12884078, registered in England & Wales). This framework is released under CC BY 4.0 — free to use, adapt, and share with attribution. "The Agent-Readiness Hierarchy" name and the Serafim Tech mark may be used to refer to this framework and accurate adaptations of it.*
