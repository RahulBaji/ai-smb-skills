# Worked example — B2B vertical SaaS

Read this for calibration on specificity, especially the guardrail math. Do not
copy its wording; copy its level of concreteness.

**Context:** A company sells warehouse inventory-accuracy software to 3PL
operators, $48k/yr ACV, 90-day implementation, competitors are legacy WMS
add-ons and spreadsheets.

## Phase 1 output

**Unspoken tax:** The industry has normalised a 90-day implementation that the
customer staffs and pays for, during which they get zero benefit and carry all
the failure risk. Operators budget for it and hate it, but no vendor removes it
because implementation revenue is 20% of vendor top line.

**Damaged metric:** Payback period. A $48k tool that delivers nothing for one
quarter has an effective 14-month payback against a 12-month budget cycle — so
it loses to "do nothing" in the CFO's model even when it wins on features.

## Phase 2 output (condensed)

**HEADLINE:** Cadence launches Zero-Quarter Onboarding — 99% inventory accuracy
in 30 days, or you pay nothing until you get it.

**SUMMARY:** For 3PL operators running 5–50 sites, Cadence now carries the
implementation risk itself: no implementation fee, no subscription billing, and
no contractual commitment until the customer's first site hits 99% cycle-count
accuracy. If day 30 arrives without that number, the clock keeps running free.

**THE CONSTRAINT:** ~$9k in implementation fees plus roughly 200 hours of
customer ops time, spent before a single benefit lands. Incumbents can't drop
it: services revenue funds their margin and their per-customer configuration is
bespoke, so their cost of a failed install is real.

**THE OFFER:** $0 up front. Billing starts the day the first site certifies at
99% accuracy on an independent cycle count. If certification takes more than 30
days from data handoff, the customer keeps the software free until it certifies.
No termination penalty in the first 90 days after certification.

**THE MECHANISM:** 340 completed 3PL installs producing a schema library that
covers 87% of incoming data formats without custom mapping; median install is
now 11 days, p90 is 19. The guarantee is priced off the p90, not the median —
the risk is real but bounded and measured.

**INTERNAL FAQ — GUARDRAILS:**
- Eligibility: 5–50 sites, one of six supported WMS platforms, named customer
  data owner. Outside that band, install variance is uncontrolled — quote
  standard terms instead.
- Customer obligations that pause the clock: data handoff completeness, sign-off
  on count schedule within 3 business days.
- Expected slip rate: 10% of installs exceed 30 days (from p90 = 19 days plus
  buffer). At 10%, mean free period is 12 extra days ≈ $1.6k of deferred
  revenue per slipped deal, against $9k of eliminated implementation cost.
- Stress case: at a 25% slip rate the offer still nets positive, because the
  services cost removed exceeds the revenue deferred. It stops working above a
  ~45% slip rate or if median install exceeds 25 days — both are monitored
  weekly and trigger a pause on the guarantee for new logos.

## Phase 3 output

| Stage | Mechanic | Metric | Expected move |
|---|---|---|---|
| Awareness | "Pay nothing until 99% accuracy" as the paid-search and trade-press hook | CPC, PR pickup | CPC down ~30%; claim is uncopyable by incumbents whose services revenue depends on the fee |
| Acquisition | No up-front spend removes capex approval; procurement path shortens to a signature | Sales cycle | 94 days → target 45; win rate vs "do nothing" is the real lift |
| Activation | First site certified at 99% on independent count | Time-to-certify, % certified ≤30d | Hold p90 ≤ 19 days; this is the single number the offer lives on |
| Retention | Weekly accuracy report + drift alerts keep sites above threshold post-certification | Post-cert accuracy, renewal | Churn risk moves from "did it install" to "did it hold" |
| Revenue | Subscription starts at certification; implementation fee eliminated entirely | ACV, payback | ACV flat at $48k, payback 14mo → 8mo, which is what actually wins the CFO |
| Referral | Ops directors who took zero budget risk and hit 99% in a month have an internal win to tell peers about | Referral rate | 3PL operators talk constantly at industry events; the story is the guarantee, not the software |

**Riskiest assumptions and cheapest tests:**
1. That 87% schema coverage holds on new logos — test by running the mapper
   against 20 prospect data samples before extending the guarantee.
2. That payback, not features, is the real objection — test with 10 lost-deal
   interviews before rebuilding pricing.
3. That legal will accept "free until certified" — get one contract redlined
   before it goes in an ad.
