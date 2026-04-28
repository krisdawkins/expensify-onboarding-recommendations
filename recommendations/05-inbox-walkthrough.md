# 05. Inbox Walkthrough Instructions Do Not Match Visuals

| Field | Value |
|---|---|
| Priority | Medium |
| Area | Documentation, In-product Guidance |
| Effort | Quick win (1 to 2 days), plus medium-term process change |
| Status | Proposed |

## Problem

During setup, the written instructions for navigating the Inbox did not align with what was shown visually on screen. Button labels, menu positions, and screen layouts referenced in the walkthrough did not match the live product interface.

## Customer impact

When guidance and visuals do not align, users question their own actions. In an onboarding context, this creates a moment of doubt: "Am I doing this wrong, or is the product wrong?"

Even small mismatches erode confidence in the product's attention to detail. Users do not always articulate what made them lose confidence; they simply abandon.

## Evidence

Direct observation during testing in April 2025. Walkthrough copy referenced UI elements that were not present in the live interface, or were located somewhere different from where the walkthrough described. (Figure: see [original-submission/](../original-submission/), Fig. 4.)

## Hypothesis on cause

The likely cause is documentation drift. The walkthrough was probably written against an earlier version of the Inbox UI, and the UI has since been updated without a corresponding refresh of the walkthrough copy and screenshots.

This is a process gap, not a content quality issue. The walkthrough is well-written. It is just out of sync with the product.

## Proposed solutions

**Quick win (1 to 2 days):** audit all walkthrough content against the current live product. Update screenshots and instructions to match. This is a documentation task, not an engineering task. One person with access to the docs CMS can complete the audit and edits in 1 to 2 days.

**Medium-term (1 to 2 months):** implement a process where walkthrough content is automatically flagged for review whenever the related product UI is updated. Could be as light as a checklist item in the engineering team's PR template ("does this change UI referenced in onboarding walkthroughs? If so, link the doc owner."). Prevents future drift between documentation and product.

**Strategic (longer-term):** consider whether some onboarding walkthrough content is best replaced with in-product micro-tours that read live UI labels, rather than static documentation that needs to be kept in sync manually. This is a build-versus-buy question with engineering investment, but eliminates the drift problem at the root.

## Expected outcome and validation

This issue has lower individual impact than the other four, but contributes to cumulative onboarding friction. When combined with [Recommendations 1, 3, and 4](./), it reinforces a perception that the onboarding experience has not been recently reviewed or maintained.

Validation plan:

1. Audit and confirm the scope of the mismatch (which walkthrough items, which UI elements).
2. After updating, manually walk through the onboarding flow on a fresh account to confirm alignment.
3. Add walkthrough freshness as a quarterly review item.
4. Track Concierge tickets that reference walkthrough confusion before and after the fix.

## Open questions

- Who owns the onboarding walkthrough content today? Is it a single team or distributed?
- What is the existing process for keeping walkthrough content in sync with UI changes?
- Are there other walkthroughs (not just Inbox) that may have the same drift issue?
- Has anyone considered moving onboarding walkthroughs into a more automated framework (in-product tours that read live labels)?

## Linked resources

- [Issue #5](../../../issues/5)
- [Original screenshot evidence](../assets/screenshots/) (figure to be added)
- [Prioritisation framework](../docs/prioritisation-framework.md)

Last updated: 27 April 2026.
