# Worked Example: Scoring a Real-ish Store

This walks one fictional merchant — **Brightwell Home**, a mid-size online homeware retailer — through the [Agent-Readiness Hierarchy](README.md), to show how the scores produce a *decision*, not just a chart.

> Licensed under CC BY 4.0. Maintained by Serafim Tech Limited · serafimtech.io

---

## The scores

Reading bottom-up: **Presence 3 · Comprehension 3 · Transactability 1 · Trust 2 · Leverage 3** — written as `3-3-1-2-3`.

| Layer | Score | Why |
| --- | :---: | --- |
| **5 · Leverage** | 3 | Promotions, bundles, and loyalty are all exposed in agent-readable form; agent traffic is tracked and attributed separately. Genuinely optimized. |
| **4 · Trust** | 2 | Returns and substitution rules are clear and machine-readable; delegated-authorization handling works but isn't yet structured to *prefer* trusted agents. Functional. |
| **3 · Transactability** | 1 | The cart accepts agent line items but **fails to return a checkout URL with a correct total** when shipping varies by region. An agent can start a purchase but can't reliably finish one. Basic, not functional. |
| **2 · Comprehension** | 3 | Catalog is clean, every variant resolves, semantic metadata and localization are all in place. Optimized. |
| **1 · Presence** | 3 | Discovery profile is reachable and parseable; a live agent endpoint is published; agentic channels are switched on. Optimized. |

---

## How to read it

**Bottleneck = Layer 3 (Transactability), at 1.**
It's the lowest layer scoring below 2. *Everything* above it is wasted until this is fixed. Brightwell's beautiful Leverage layer (5 = 3) earns nothing in practice, because an agent that can't complete checkout never reaches a promotion.

**Overall readiness = Layer 2 (Comprehension).**
That's the highest layer scoring ≥2 with no gap beneath it. Presence (3) and Comprehension (3) form an unbroken floor — but the chain breaks at Transactability (1), so readiness stops there. Brightwell is, in effect, *a store agents can find and understand but cannot buy from.*

This is the trap the hierarchy is built to expose: **the headline scores look great** (three 3s!) but the store scores as Layer-2-ready, because readiness is gated by your first weak floor, not your best layer.

---

## The fix list this produces

| Priority | Layer | Move | Action |
| :---: | --- | :---: | --- |
| **1** | 3 · Transactability | 1 → 2 | Make checkout return a working URL with a correct total in every region, including variable shipping and tax. **This single fix raises overall readiness from Layer 2 to Layer 5.** |
| 2 | 4 · Trust | 2 → 3 | Structure delegated-authorization signals so trusted agents are preferred, not merely accepted. |
| 3 | 5 · Leverage | hold at 3 | Already optimized — protect it; no spend until Layer 3 is fixed. |

Note the leverage: because the layers gate each other, fixing one weak floor (Transactability) unlocks the entire stack above it. **A 1-point fix at the bottom is worth more than a 1-point gain anywhere else.**

---

## The general rule, restated

- Find the lowest score below 2. That's the bottleneck. Fix it first.
- Your overall readiness is the highest unbroken layer ≥2.
- Spending above your bottleneck is spending you can't yet collect on.

---

*© 2026 Serafim Tech Limited. Released under CC BY 4.0 — free to use, adapt, and share with attribution.*
