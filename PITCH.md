# Spectra Nova for TELUS

**One screen. Five faults. No second visit.**

A win for the customer. A win for the tech. A win for TELUS.

---

## The problem we're paying for today

A residential WiFi complaint resolves to one of five things:
**ISP line · modem · channel congestion · signal at the complaint location · customer device.**

No tech has a single tool that reads all five in under five minutes. They improvise with `netsh`, `ipconfig`, consumer apps, and tribal knowledge — then leave with a guess.

When the guess is wrong, the truck goes out a second time. **At $250 per truck roll, even a 5 % cut in repeat visits across a province-sized field force lands in seven figures a year.**

---

## What Spectra Nova does

**One screen. Live data. Ten panels.**
RF spectrum across all three bands · network list with signal history · channel congestion analysis · ping / speed / bufferbloat · room-by-room coverage walk · subnet device scan · network tools · history · WiFi Health Check (a single 0–100 score with a customer-facing branded HTML report).

**An assistant grounded in TELUS-specific knowledge.**
338 curated entries across 16 categories — PureFibre plans, modems, devices, networking concepts. The assistant cites live readings, never invented ones. **Zero hallucination on matched queries**, verified against a 540-cell regression matrix on every change.

**100 % offline by default.** Audited 8-endpoint allowlist. Passes a privacy review in one meeting.

**Owned, not rented.** Source, KB, and CI pipeline transfer with the license. No SaaS dependency. No surprise data residency. No third-party telemetry. Built in-house, not subscribed-to.

---

## Win × Win × Win

|  | **Customer** | **Technician** | **TELUS** |
|---|---|---|---|
| **Speed** | Less time on the call | Less guessing | Shorter handle time |
| **Confidence** | Sees real numbers, not "trust me" | Diagnosis with citations | Lower escalation rate |
| **Closure** | Branded report after every visit | Knows what was changed and why | Consistent ticket documentation |
| **Repeat visits** | One trip, not two | No "I missed it last time" call-backs | **Direct truck-roll cost reduction** |
| **Training** | Same quality of service from any tech | Senior-level reasoning embedded in the tool | Faster new-hire ramp; tribal knowledge captured |

---

## The financial story

**Estimate, not forecast.** We don't have your operations data. Here's the model, anchored where possible in TELUS public reporting and industry benchmarks.

**Annual truck-roll savings = N × T × 12 × R × I × $250**

- `N` — your field tech count *(TELUS reports ~25,200 Canadian employees in 2025; field-tech subset is a fraction)*
- `T` — truck rolls per tech per month *(industry typical: 20–40)*
- `R` — current repeat-visit rate *(industry typical: 15–25%)*
- `I` — repeat-visit reduction Spectra Nova delivers — **the pilot measures this**
- `$250` — TELUS-aligned truck-roll cost *(industry range $150–$600)*

**Illustrative — N = 1,000, T = 30, R = 20%:**

- `I` = 5% (sensitivity): **$900 K / year on truck rolls alone**
- `I` = 10% (conservative): **$1.8 M / year**
- `I` = 25% (stretch): **$4.5 M / year**

Savings scale linearly with `N`. A 2,000-tech fleet doubles those numbers.

**Truck rolls only.** Layer on handle-time and escalation reduction — both pilot-measured — and the model compounds. **Whatever `I` turns out to be, plug it back in. The answer is yours, not ours.**

Spectra Nova is instrumented end-to-end for the measurement: every query, every diagnostic, every export logged for the post-pilot review.

---

## Why not just give techs an LLM?

LLMs hallucinate device specs, plan tiers, signal thresholds. Spectra Nova can't — the curated KB and structured analyzers don't generate numbers, they cite them.

|  | **Spectra Nova** | **On-device LLM** |
|---|---|---|
| Hallucination on matched queries | Zero | Real risk |
| Determinism | Regression-testable | Stochastic |
| Privacy | 100 % offline, 8 audited endpoints | Same |
| Update cycle | Add a KB entry, ship it | Fine-tune (expensive) or re-prompt (fragile) |
| Audit story | "540 cells passing on every commit" | "Trust me" |

If you want LLM-grade reasoning for novel queries, **a Claude API integration is already built in**. Per-tech opt-in via API key. Rate-limited and audit-logged. **Off by default** — entirely Spectra Nova's curated KB until a tech opts in.

---

## The integration upside

What ships **today, standalone** is the field tool described above. Three integration tiers compound the value as TELUS opens access — same architecture, same KB, same UI surface, multiplied ROI.

### Tier 1 — Modem-embedded *(the destination)*

With a lightweight firmware agent on the modem, Spectra Nova streams live diagnostics — CPU temperature, modulation profile, line attenuation, SNR margin, error counters — straight into the field tool. **"Walk in, plug in, locate, solve."** Many visits resolve before the tech finishes setup.

### Tier 2 — Backend-connected *(the next step)*

With access to TELUS provisioning, ONT health, account flags, neighborhood-outage signals, and modem fleet inventory, the assistant retrains on TELUS-specific data and handles **line-level issues the customer side can't reveal**: account provisioning gaps, plan-tier mismatches, regional ISP-side outages, ONT silent-fail patterns. The tech walks in already knowing whether the issue is local or upstream.

### Tier 3 — Field tool *(the foundation, already built)*

WiFi diagnostic with curated KB. Tech sees what's in the room. Bot answers from grounded readings. Zero hallucination, fully offline. **Pilot-ready today.**

---

Each tier shares infrastructure. **TELUS pays once for the architecture; the integrations multiply the savings.**

---

## Status

- **v1.2.0** — signed `.app` for macOS, signed `.exe` for Windows
- 237 unit tests passing on every push (test scaffolding actively expanding)
- 540-cell scenario matrix with regression detection
- 9 supported languages
- Built solo. Independent. Ready to license.

Architecture and methodology available on request.

---

## The ask

**Four weeks. One truck crew. A control group.** Instrument the queries and the outcomes. Measure first-time-fix rate and truck-roll time against the control. **Decide from the data.**

---

**Kevin Madson** — [kevinmadson@protonmail.com](mailto:kevinmadson@protonmail.com)
