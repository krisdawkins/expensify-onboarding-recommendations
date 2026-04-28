# 02. Cashback Messaging Creates Regional Bias

| Field | Value |
|---|---|
| Priority | Highest |
| Area | Customer Trust, Localisation |
| Effort | Quick win (1 day), plus medium-term geo-filtering and strategic localisation |
| Status | Proposed |

## Problem

Expensify promotes cashback rewards for Expensify Card purchases, but the messaging highlights benefits available only on US purchases. As a UK-based user, I saw promotional value that I am not eligible for, with no labelling or filtering to indicate that.

This creates an immediate sense of exclusion. Instead of feeling rewarded, the messaging creates a perception that the product is optimised for a different user segment.

## Customer impact

Perceived fairness heavily influences customer trust. When regional users feel secondary to the primary market, it reduces product loyalty and increases openness to competitor solutions offering more locally relevant benefits.

For a company expanding internationally, this is a retention risk that compounds over time. The first encounter with US-only messaging seeds a template the user uses to interpret subsequent UX choices.

## Evidence

Direct observation during testing in April 2025. Cashback messaging appeared in the dashboard area of New Expensify shortly after sign-up, with no indication that the offer was region-specific. Screenshot evidence captured at the time. (Figure: see [original-submission/](../original-submission/), Fig. 1.)

## Hypothesis on cause

The likely cause is that the cashback feature was built for the US Expensify Card programme and the marketing surface inherited that scope without geographic filtering at the presentation layer. The feature itself is region-specific. The messaging is not.

This is a common pattern when a US-headquartered product expands internationally: the substance of features is regionalised, but the messaging surface ships globally.

## Proposed solutions

**Quick win (1 day):** add a clear label to all cashback messaging: "This offer is available in the US only." One line of copy, deployable in days, eliminates the confusion immediately.

**Medium-term (2 to 4 weeks):** geo-filter promotions so users only see offers relevant to their market. UK users see UK-relevant benefits; US users see US benefits. Requires backend logic for region detection and content selection, but eliminates the problem entirely rather than mitigating it.

**Strategic (1 to 3 quarters):** build a localised reward programme for non-US markets. Even modest cashback or partner offers in the UK or EU would shift the perception from "this product is not for me" to "this product understands my market." This is a business decision, not a UX one, but the UX evidence supports the case.

## Expected outcome and validation

If Expensify's non-US user base represents 20 to 30 percent of total users (illustrative), and perceived regional bias increases churn by even 2 to 3 percent, the revenue impact across international markets could be significant, particularly as competitors like Pleo (Europe) and Spendesk (Europe) offer fully localised experiences.

Both the 20 to 30 percent figure and the 2 to 3 percent churn impact are illustrative.

Validation plan:

1. Pull actual non-US user share from existing analytics.
2. Pull retention curves segmented by region.
3. Run a short survey of recent non-US sign-ups asking about perception of regional relevance.
4. After shipping the quick-win label, measure click-through and dismissal rates on the cashback message by region.
5. After geo-filtering ships, measure overall promotional engagement among non-US users versus the previous baseline.

## Open questions

- What proportion of non-US users actually engage with cashback messaging today, before any change?
- Are there active competitor benchmarks for localised reward programmes that the team has already evaluated?
- Is region detection already available in the messaging layer, or would this require new instrumentation?
- Are there other US-only promotions exposed to non-US users that this fix should also cover (Expensify Card sign-up incentives, partner offers, referral programmes)?

## Linked resources

- [Issue #2](../../../issues/2)
- [Original screenshot evidence](../assets/screenshots/) (figure to be added)
- [Prioritisation framework](../docs/prioritisation-framework.md)

Last updated: 27 April 2026.
