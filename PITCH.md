# Spectra Nova for TELUS

**One screen. Five faults. No second visit.**

Customers win. Techs win. TELUS wins.

---

## The problem we're paying for today

A residential WiFi complaint resolves to one of five things:
**ISP line · modem · channel congestion · signal at the complaint location · customer device.**

No tech has a single tool that reads all five in under five minutes. They improvise with `netsh`, `ipconfig`, consumer apps, and tribal knowledge, then leave with a guess.

When the guess is wrong, the truck goes out a second time. **At $250 per truck roll, even a 5 % cut in repeat visits across a province-sized field force lands in seven figures a year.**

---

## What Spectra Nova does

**In under five minutes, the tech sees:** signal at every room, channel congestion on every band, real download and upload speeds, bufferbloat under load, every device on the subnet. All of it distilled into a single 0–100 WiFi Health score with a customer-facing branded HTML report. **One screen. Ten panels. Zero modem-GUI dance.**

**An assistant that reads the live network.** When a tech asks *"why is it slow?"*, the bot pulls the current RSSI, the channel congestion percentage, the last speed-test result, and the dropped-device history, then answers with those exact numbers cited inline. The numbers it cites are the ones reading off the radio at the moment the question is asked. Backed by 338 curated TELUS-specific KB entries across 16 categories. **Zero hallucination on matched queries**, verified against a 540-cell regression matrix on every change.

**100 % offline by default.** Audited 8-endpoint allowlist. Passes a privacy review in one meeting.

**Owned, not rented.** Source, KB, and CI pipeline transfer with the license. No SaaS dependency. No surprise data residency. No third-party telemetry.

---

## Win × Win × Win

|  | **Customer** | **Technician** | **TELUS** |
|---|---|---|---|
| **Confidence** | Sees real numbers, not "trust me" | Diagnosis with citations, not guesses | Lower escalation rate · consistent documentation |
| **Closure** | Branded report after every visit | Walks out knowing what changed and why | Shorter handle time · fewer callbacks |
| **Repeat visits** | One trip, not two | No "I missed it last time" tickets | **Direct truck-roll cost reduction** |

> *Tuesday afternoon. The customer has called three times this month about the same disconnect. The tech opens Spectra Nova, runs the Health Check, and walks out twenty minutes later with a printed report explaining exactly what was changed and why. **The customer doesn't call back.***

---

## The financial story

**Estimate, not forecast.** We don't have your operations data. Here's the model, anchored where possible in TELUS public reporting and industry benchmarks.

**Annual truck-roll savings = N × T × 12 × R × X × $250**

- `N`: your field tech count *(TELUS: ~25.2K Canadian employees; field-tech subset is a fraction)*
- `T`: truck rolls per tech per month *(industry typical: 20–40)*
- `R`: current repeat-visit rate *(industry typical: 15–25%)*
- `X`: repeat-visit reduction Spectra Nova delivers. **The pilot measures this.**
- `$250`: TELUS-aligned truck-roll cost *(industry range $150–$600)*

**Illustrative: N = 1,000, T = 30, R = 20%**

- `X` = 5% (sensitivity): **$900 K / year on truck rolls alone**
- `X` = 10% (conservative): **$1.8 M / year**
- `X` = 25% (stretch): **$4.5 M / year**

Savings scale linearly with `N`. A 2,000-tech fleet doubles those numbers.

**Truck rolls only.** Layer on handle-time and escalation reduction (both pilot-measured) and the model compounds. **Whatever `X` turns out to be, plug it back in. The answer is yours.**

Spectra Nova is instrumented end-to-end for the measurement. Every query and diagnostic is logged, ready for the post-pilot review.

---

## Why not just give techs an LLM?

LLMs hallucinate device specs, plan tiers, signal thresholds. Spectra Nova can't. Its curated KB and structured analyzers cite numbers; they never invent them.

|  | **Spectra Nova** | **On-device LLM** |
|---|---|---|
| Hallucination on matched queries | Zero | Real risk |
| Privacy | 100 % offline, 8 audited endpoints | Same |
| Update cycle | Add a KB entry, ship it | Fine-tune (expensive) or re-prompt (fragile) |
| Audit story | 540 cells passing on every commit | Opaque reasoning, no audit trail |

---

## Or run Claude inside Spectra Nova

**The Anthropic API integration is already wired.** Paste an API key and Claude takes over as the assistant. The *same live network context* flows through: RSSI, congestion, speed, device history. Sensitive details masked on the way out. Rate-limited. Audit-logged. **Off by default**, per-tech opt-in.

For TELUS, that's **two deployment paths shipping today**: standalone (curated KB, fully offline, zero cloud) or Claude-augmented (frontier reasoning, customer data masked). One install, one license, one fleet. Your techs choose.

---

## The integration upside

What ships today is the field tool described above. As TELUS opens access, three integrations deepen the value without changing the architecture or the surface area.

### Tier 1: Modem-embedded *(the destination)*

With a lightweight firmware agent on the modem, Spectra Nova streams live diagnostics straight into the field tool: CPU temperature, modulation profile, line attenuation, SNR margin, error counters. **"Walk in, plug in, locate, solve."** Many visits resolve before the tech finishes setup.

### Tier 2: Backend-connected *(the next step)*

With access to TELUS provisioning, ONT health, account flags, neighborhood-outage signals, and modem fleet inventory, the assistant retrains on TELUS-specific data and handles **line-level issues the customer side can't reveal**: account provisioning gaps, plan-tier mismatches, regional ISP-side outages, ONT silent-fail patterns. The tech walks in already knowing whether the issue is local or upstream.

### Tier 3: Field tool *(the foundation, already built)*

WiFi diagnostic with curated KB. Tech sees what's in the room. Bot answers from grounded readings. Zero hallucination, fully offline. **Pilot-ready today.**

---

Each tier shares infrastructure. **TELUS pays once for the architecture; the integrations multiply the savings.**

---

## Status

- **v1.2.0**: signed `.app` for macOS, signed `.exe` for Windows
- 237 unit tests passing on every push (test scaffolding actively expanding)
- 540-cell scenario matrix with regression detection
- 9 supported languages
- Built solo. Independent. Ready to license.

Architecture and methodology available on request.

---

## Built from the field

I'm Kevin Madson. Nine years as a field technician before this.

*Currently applying for the Senior Business Analyst role at TELUS.*

Every analyzer, every KB entry, every *"why does this break this way"* assumption in Spectra Nova traces back to a real customer visit. A real escalation chain. A real *"I knew it, but I couldn't prove it"* moment. **Built by a tech, for techs.**

The bot doesn't know what it's like to walk into a customer's house at 4 PM on a Friday. **The person who built it does.**

---

## The ask

**Four weeks. One truck crew. A control group.** Instrument the queries and the outcomes. Measure first-time-fix rate and truck-roll time against the control. **Decide from the data.**

Email below. Happy to walk through the architecture, the regression matrix, or the integration roadmap in thirty minutes.

---

**Kevin Madson** · [kevinmadson@protonmail.com](mailto:kevinmadson@protonmail.com)
