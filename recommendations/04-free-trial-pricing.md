# 04. Free Trial Pricing Communication Is Unclear

| Field | Value |
|---|---|
| Priority | High |
| Area | Billing Transparency, Onboarding |
| Effort | Quick win (1 day), plus medium-term pricing surface |
| Status | Proposed |

## Problem

I initially believed Expensify was free for individual users. Repeated references to a "30-day free trial" during onboarding created uncertainty about future costs.

It was unclear whether I would be charged after 30 days, what the pricing tiers were, or whether individual use remained free indefinitely.

## Customer impact

Pricing confusion weakens trust quickly, particularly for users evaluating multiple expense tools. If a user does not understand what they will pay, they are less likely to invest time in setup and adoption.

This is especially critical during a trial period when the product needs to demonstrate value before asking for payment. Trial users who are unsure about pricing are also more likely to bail before the trial expires, simply to avoid the perceived risk of being charged.

## Evidence

Direct observation during testing in April 2025. The "30-day free trial" framing appeared in onboarding messaging without an accompanying explanation of what happens after the trial, what the paid tier costs, or whether individual use remains free. (Figure: see [original-submission/](../original-submission/), Fig. 3.)

## Hypothesis on cause

The likely cause is that the free-trial framing was designed for the team and enterprise pricing surface, where a 30-day trial of paid features makes sense. When applied to an individual user signing up for personal expense tracking, the same framing creates ambiguity.

This is a copy and information-architecture issue, not a pricing-policy issue. Expensify's pricing structure may be sound. The communication of it is what is breaking down.

## Proposed solutions

**Quick win (1 day):** add clear pricing messaging at sign-up. Suggested copy variants depending on user type:

- For individual users: "Free for individuals. No credit card required."
- For team sign-ups: "Free 30-day trial. Team plans start at $5 per user per month after your trial. You will not be charged until you choose a paid plan."

One line of clear copy at the relevant decision point eliminates the ambiguity.

**Medium-term (1 to 2 months):** add a pricing comparison page accessible from the onboarding flow, showing exactly what is free, what is paid, and what happens after the trial. Include a "you will not be charged" reassurance for individual users. Link to it from the "30-day free trial" reference.

**Strategic:** consider revisiting how Expensify segments individual users from team users at sign-up. If individual users are routed to a different onboarding flow (see [Recommendation 3](03-workspace-setup.md)), the trial framing would not appear in their flow at all.

## Expected outcome and validation

Unclear pricing is consistently cited in industry research as a top reason users abandon SaaS trials. (Industry references vary; treat as directional.)

If 15 percent of trial users are confused about pricing and 20 percent of those do not convert because of the confusion, that is a 3 percent reduction in trial-to-paid conversion. Both percentages are illustrative.

Validation plan:

1. Pull trial-to-paid conversion rate from existing analytics.
2. Pull Concierge tickets containing the terms "free trial", "charge", "billing", "price". Quantify the proportion that indicate confusion versus genuine pricing-policy disagreement.
3. Run a short post-trial survey of recent trial expirations, including a question on whether pricing was clear.
4. After shipping the quick-win copy, measure conversion rate change among new sign-ups.
5. After the pricing comparison page ships, measure click-through and time-on-page from the onboarding flow.

## Open questions

- What is the current trial-to-paid conversion rate, and how does it segment by user type (individual, team, enterprise)?
- Are individual users genuinely free indefinitely, or is the free tier feature-limited in ways that need to be communicated?
- Has the team A/B-tested pricing copy variants in the past? If so, what was the result?
- How does Expensify's pricing clarity compare to competitor sign-up flows (Brex, Ramp, Pleo, Soldo)?

## Linked resources

- [Issue #4](../../../issues/4)
- [Original screenshot evidence](../assets/screenshots/) (figure to be added)
- [Prioritisation framework](../docs/prioritisation-framework.md)

Last updated: 27 April 2026.
