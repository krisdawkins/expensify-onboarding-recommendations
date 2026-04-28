# Limitations

What this analysis is not. Posted up-front because owning the limitations of work is faster than having someone else find them.

## Sample size

A single tester, a single persona, two hours of use. This is preparation for a conversation, not a peer-reviewed study.

The 5 issues identified are real friction points encountered by one user during one window of testing. Whether they generalise to the broader user base is an empirical question that the [30-day plan](30-day-plan.md) starts to answer.

## Persona scope

The persona was a first-time UK-based individual user setting up Expensify for personal expense tracking. That is one slice. The same friction points may register differently for:

- Enterprise admins onboarding a workspace for hundreds of users.
- Finance leads evaluating Expensify against an incumbent tool.
- Multi-country teams configuring policies across regions.
- Existing users upgrading from a free trial.
- Mobile-only users who never touch the web platform.

A complete onboarding analysis would test against several of these in addition. This repo does not.

## Numbers are illustrative

Throughout this repo, business-impact figures are flagged as illustrative. Specifically:

- The **53 percent abandonment** statistic referenced in [Recommendation 1](../recommendations/01-mobile-load-time.md) draws on Google's research on mobile load times. It is a directional reference, not a precise prediction of Expensify's actual abandonment rate.
- The **50,000 new users per month** assumption used in business-impact calculations is an illustrative placeholder. The real number is private to Expensify.
- The **20 to 30 percent non-US user proportion** in [Recommendation 2](../recommendations/02-cashback-us-only.md) is an estimate. Actual share by region is private.
- The **cumulative drop-off model** in [the prioritisation framework](prioritisation-framework.md) compounds illustrative assumptions and produces an illustrative outcome (~21 percent drop-off). It is intended to show shape, not to claim precision.

In the role, the first action would be to replace these placeholders with real data. The recommendations themselves stand or fall on their own merits, not on the impact numbers.

## Surface coverage

I tested Chrome on macOS and iOS. I did not test:

- Android.
- Other desktop browsers (Firefox, Safari, Edge).
- iOS or Android tablets.
- The web app on mobile breakpoints.
- The Concierge experience across multiple interactions.
- Card transactions, integrations beyond auth screens, or Expensify Travel.

The omitted surfaces likely contain their own friction patterns.

## Time

Two hours is enough to identify first-impression friction. It is not enough to identify the friction patterns that emerge in week 2 of use, or in workspace configurations more complex than the default.

## Comparative framing

I came in with prior Concur experience as my benchmark. That benchmark shaped what I noticed and what I did not. A tester from a different background (Brex/Ramp, Pleo, no expense tool at all) would surface different patterns.

## The honest summary

Treat this repo as a starting point for a conversation, not a finished diagnosis. The recommendations are real recommendations grounded in real observations. The numbers around them are placeholders. The validation work in [the 30-day plan](30-day-plan.md) is what would turn this into a finished diagnosis.

Last updated: 27 April 2026.
