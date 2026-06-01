# Per-Layer Objective Checks

The maturity scale is only as honest as the evidence behind it. Self-assessed scores invite grade inflation — *everyone* thinks their catalog is a 2. These checks turn each score into something you can **pass or fail**, not just claim.

Rule of thumb for every layer: **a score is whatever the failing agent would grade you, not what your demo shows.** If any check at a level fails, you have not reached that level.

> Licensed under CC BY 4.0. Maintained by Serafim Tech Limited · serafimtech.io

---

## Layer 1 · Presence — *Can an agent find and reach me at all?*

| Score | You reach this level only if… |
| :---: | --- |
| **1** | A discovery profile exists somewhere an agent could plausibly find, but it's incomplete, stale, or not machine-parseable. |
| **2** | An agent can retrieve a parseable discovery profile **and** hit a live agent endpoint that responds correctly, through at least one enabled agentic channel. |
| **3** | All of 2, **and** your presence is structured/published such that an agent surfaces you among the first candidates for a relevant intent (not just *reachable*, but *preferred at discovery*). |

---

## Layer 2 · Comprehension — *Can it understand what I sell?*

| Score | You reach this level only if… |
| :---: | --- |
| **1** | A catalog is exposed, but variants don't reliably resolve, structured data is partial, or key attributes are missing/ambiguous. |
| **2** | An agent can resolve **any** product to the correct variant (size/colour/config), read structured data for price, availability, and core attributes, and get the right answer in each supported locale. |
| **3** | All of 2, **and** semantic metadata is rich enough that an agent can match your product to a *described need* ("quiet fan for a nursery") — comprehension good enough to win comparison, not just survive it. |

---

## Layer 3 · Transactability — *Can an agent actually buy?*

| Score | You reach this level only if… |
| :---: | --- |
| **1** | An agent can add items to a cart, but checkout fails, totals are wrong, or no usable checkout URL is returned in some valid cases. |
| **2** | An agent can submit line items, receive a **correct total** (including tax and shipping for every supported region), get a **working checkout URL**, and reach a payment handler and a valid fulfillment option — end to end, repeatably. |
| **3** | All of 2, **and** the transaction path is structured so a competent agent completes it faster / with fewer failures at your store than at a comparable merchant. |

---

## Layer 4 · Trust — *Can the transaction be trusted?*

| Score | You reach this level only if… |
| :---: | --- |
| **1** | Some trust handling exists (e.g. you accept delegated payment) but returns, substitution, or authorization rules are opaque or inconsistent to an agent. |
| **2** | Delegated authorization is handled correctly; returns, refunds, and substitution policy are **machine-readable and consistently applied**; an agent can determine your dependability before transacting. |
| **3** | All of 2, **and** you publish a Know-Your-Agent posture that lets you *prefer* verified/trusted agents — trust is a signal you act on, not just a box you clear. |

> **Note — Trust may be market-specific.** Unlike the other layers, the trust threshold is shaped by local norms and law (payment preferences, data sovereignty). A store can legitimately be Trust-3 in one market and Trust-1 in another. Score Trust **per market** if you operate across regions with different expectations.

---

## Layer 5 · Leverage — *Can I capture value and learn?*

| Score | You reach this level only if… |
| :---: | --- |
| **1** | Some agent-facing value exists (e.g. a promotion an agent could read) but there's no attribution, no observability, and no feedback loop. |
| **2** | Promotions, loyalty, and bundles are exposed in agent-readable form **and** agent-driven activity is attributed and observable separately from human traffic. |
| **3** | All of 2, **and** you close the loop: agent-interaction data actively informs pricing, assortment, or new monetization — you're *learning from* agents, not just *serving* them. |

---

## Why Comprehension (2) and Leverage (5) are the optimization edge

The framework singles out these two layers as where a focused smaller merchant beats a bigger, sloppier one. The reason is asymmetry:

- **Comprehension is cheap to perfect and big catalogs are messy.** Clean, fully-resolving, semantically rich product data is mostly *discipline*, not budget — and large retailers, with millions of SKUs and legacy systems, are structurally bad at it. A small merchant can reach 3 here that a giant can't.
- **Leverage rewards cleverness over scale.** Smart agent-readable bundles, attribution, and feedback loops are design decisions, not spend. Scale doesn't help; insight does.

Presence, Transactability, and Trust are mostly *table stakes* — you clear them to play. Comprehension and Leverage are where you actually win.

---

*© 2026 Serafim Tech Limited. Released under CC BY 4.0 — free to use, adapt, and share with attribution.*
