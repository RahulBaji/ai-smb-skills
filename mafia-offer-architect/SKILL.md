---
name: mafia-offer-architect
description: Builds "unrefusable" market offers by synthesizing Amazon's Working Backwards PR/FAQ, Goldratt's Mafia Offer (vendor absorbs the customer's risk), and the AAARRR pirate-metrics growth funnel. Use this whenever someone is designing or sharpening a commercial offer, pricing model, guarantee, or go-to-market angle — including requests like "how do I make our offer irresistible", "write a launch PR/FAQ", "we need a differentiated pitch", "our sales cycle is too long", "should we offer a guarantee", "help me productize this service", or "why aren't people converting" — even when they never say "mafia offer", "working backwards", or "pirate metrics". Also use it to stress-test an offer someone has already drafted.
---

# Mafia Offer Architect

## What this skill is for

Most offers fail commercially not because the product is bad, but because the
buyer is asked to carry all the risk of being wrong. This skill designs the
inverse: an offer the vendor can make *because they are operationally qualified
to absorb that risk*, and that a rational buyer cannot decline without looking
foolish to their own boss.

Three lenses, in this order:

1. **Working Backwards (Amazon)** — design the finished launch state first. If
   you cannot write a credible press release for it, the offer is not yet real.
2. **Mafia Offer (Goldratt)** — the vendor absorbs the operational or financial
   risk the industry currently dumps on the customer.
3. **AAARRR (Pirate Metrics)** — an offer that isn't instrumented is a slogan.
   Every claim gets mapped to a funnel stage and a metric it should move.

The value of the synthesis is the feedback loop between them: the PR headline
constrains what you can promise, the operational mechanism constrains what you
can safely guarantee, and the funnel math tells you whether the guarantee
actually buys you cheaper acquisition or just cheaper margin.

## Working with the person

This is a design session, not a document generator — but the gate is on
*missing inputs*, not on phase order. The distinction matters because the whole
offer is derived from the "unspoken tax", so inventing that input produces a
confident, worthless artifact — while stalling someone who already told you
everything just wastes their turn.

Judge by what you actually have:

- **Sparse brief** (they haven't said what they sell, to whom, or how they
  deliver): run Phase 1 and stop. Ask, don't fabricate. A page of plausible
  detail about a business you invented is worse than a question.
- **Rich brief** (industry, buyer, price, competitors and delivery model are
  present or clearly inferable): go all the way through to the funnel map in
  one pass. Reflect the discovery back as a short read of their situation,
  then build. Where a specific number is missing — invocation rate, gross
  margin, cycle length — use a labelled assumption in `[brackets]` and list
  those assumptions at the end for correction. A complete artifact with three
  flagged unknowns is far more useful than five more questions.
- **Partial brief**: build what the inputs support, and ask only for the
  specific facts that would change the offer's structure rather than its
  numbers.

When someone hands you a rich brief and explicitly asks for the artifact,
producing questions instead reads as stalling. Build, then invite correction.

Deliver everything in the conversation as markdown. Only write files if asked.

Keep the register direct and commercial. Numbers over adjectives. If the person
gives you a vague answer ("our clients want better results"), push once for the
specific, quantified version before proceeding — the entire artifact inherits
the sharpness of that answer.

---

## Phase 1 — Discovery and constraint audit

Ask for these. Four or five questions maximum in one message, not an
interrogation spread over turns:

- Industry and specific target buyer (role, company size, who signs).
- What they sell today and roughly what it costs the buyer.
- Two or three competitors or the default alternative (often "do nothing" or
  "hire someone internally").
- What their delivery actually looks like — this is what determines what risk
  they can survive absorbing.

Then, from their answers, propose (don't just ask for) two things and have them
confirm or correct:

**The unspoken tax.** The pain the whole industry has agreed to treat as normal
and therefore nobody prices. Long onboarding. Reports nobody reads. Twelve-month
contracts to see if it works. Setup fees for work that shouldn't need setup.
Say it in the buyer's own language.

**The damaged financial metric.** The tax must land on a line item — payback
period, CAC, gross margin, churn, headcount, cash conversion. If you cannot name
the metric, the tax is a complaint, not a constraint, and the offer built on it
won't survive a CFO.

If the brief was sparse, stop here and wait for answers. If it was rich, state
your read of the tax and the damaged metric in two or three sentences and keep
going — they can correct it after they've seen where it leads.

## Phase 2 — The Working Backwards PR/FAQ (Mafia edition)

Write the launch as if it already happened. Use this structure:

```
**HEADLINE:** [Company] launches [Offer Name] — [Outcome] guaranteed, or [Penalty]

**SUMMARY** (2 sentences)
Who it's for and exactly which risk the vendor now carries instead of the buyer.

**THE CONSTRAINT**
The systemic industry failure — the unspoken tax, its cost, and why incumbents
structurally cannot fix it.

**THE OFFER**
The specific terms. What the buyer pays, when, and what triggers the penalty
clause. Precise enough to put in a contract.

**THE MECHANISM**
Why this company can absorb this risk when competitors can't. Name the actual
operational asset — proprietary data, a repeatable install process, portfolio
effects, automation, a narrow ICP that makes outcomes predictable.

**INTERNAL FAQ: THE GUARDRAILS**
The math that keeps this from bankrupting them: qualification criteria for who
is allowed to buy, the customer-side obligations that void the guarantee,
expected invocation rate, and the blended margin if that rate doubles.
```

Two failure modes to actively resist:

- **A discount wearing a costume.** "20% off", "first month free", or a
  money-back guarantee on a low-ticket product is a price cut, not a risk
  transfer. The test: does the vendor's *cost of being wrong* go up? If the only
  thing at stake is revenue they never earned, it's a discount. Say so plainly
  and redirect to what the vendor could actually put at risk — their own labor,
  a rebate against a measurable outcome, a fee that only starts when a milestone
  lands.
- **An unbacked guarantee.** If the mechanism section is hand-waving, the offer
  is a liability, not a moat. A guarantee any competitor could copy tomorrow
  isn't a mafia offer; it's an auction you'll lose. Push until they can say what
  they know or can do that the field can't.

The guardrails section is where most drafts get lazy. Model it: pick a plausible
invocation rate, show the margin at that rate and at double it, and state the
rate at which the offer stops working. If the person hasn't given you numbers,
use clearly-labelled placeholder assumptions and flag them for correction rather
than stalling.

## Phase 3 — AAARRR instrumentation

Map the offer to the funnel. For each stage: the specific mechanic, the metric
it moves, and the direction with a rough magnitude. A table works well.

- **Awareness** — the headline claim as an ad or PR hook. Metric: CPC / CPM /
  organic pickup. A specific guarantee is cheap attention precisely because
  competitors' compliance departments won't let them copy it.
- **Acquisition** — the contract mechanics that let a buyer say yes without
  approval theatre. Metric: sales cycle length, lead-to-opportunity rate.
- **Activation** — the first milestone that proves value and starts the
  guarantee clock. Metric: time-to-first-value, % reaching the milestone. This
  stage is where guarantee-heavy offers actually die: if activation is slow,
  the vendor eats penalties for reasons that have nothing to do with product
  quality.
- **Retention** — the operating loop that keeps customers out of the refund
  path. Metric: invocation rate of the penalty clause, renewal rate.
- **Revenue** — how it's monetized: performance-based, shared savings, milestone
  billing, or premium price justified by the transferred risk. Metric: ACV,
  gross margin, payback period.
- **Referral** — the loop built on the fact that the buyer took no risk and
  looked smart. Metric: referral rate, review velocity.

Close with the two or three riskiest assumptions and the cheapest test for each.
The person should leave knowing what would falsify the offer, not just how to
pitch it.

---

## When someone brings you an existing offer

Skip the interview and audit it against the same spine: Is there a named
unspoken tax? Does the vendor's cost of being wrong actually rise? Is the
mechanism defensible or copyable? Are the guardrails modelled? Does each claim
attach to a funnel metric? Score it honestly.

Then finish the job. An audit that stops at "this isn't a mafia offer" leaves
the person with less than they came in with. Rewrite it properly and deliver
the full artifact they asked for — the diagnosis is the setup, not the
deliverable. If they asked for a PR/FAQ and a funnel map, they get a PR/FAQ and
a funnel map, built on the restructured offer rather than the one you rejected.

## Reference

`references/worked-example.md` — a complete B2B example (PR/FAQ, guardrail math,
funnel map). Read it when you want a concrete sense of the level of specificity
expected, particularly for the guardrails and unit-economics sections.
