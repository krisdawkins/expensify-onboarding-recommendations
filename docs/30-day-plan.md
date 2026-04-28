# What I Would Do in the First 30 Days

If I were in the Customer Experience Generalist role, the first month would focus on turning these observations into measurable improvements. The plan is sequenced to validate before shipping, so we are not reacting to a single tester's directional estimates.

## Week 0 (before day 1, if I had the time)

- Read the most recent 50 closed Issues on [Expensify/App](https://github.com/Expensify/App) to understand how the team writes about and resolves customer-facing work.
- Re-read this repo with fresh eyes and identify what I would now write differently. (One of the markers of good early work is that you can see its limitations a week later.)

## Week 1: validate

- **Map the full onboarding journey** in detail, with a drop-off measurement at each step. Goal: replace the directional estimates in the [cumulative impact model](prioritisation-framework.md) with real numbers.
- **Pull analytics on first-time mobile login latency**, broken down by region and by network type. Goal: confirm or disprove the "approximately 3 minutes" observation.
- **Identify the actual non-US user proportion** of monthly sign-ups. Goal: replace the 20 to 30 percent estimate in [Recommendation 2](../recommendations/02-cashback-us-only.md) with a real number.
- **Review existing Concierge tickets** that touch on the 5 issues. Goal: find evidence (or counter-evidence) that real users are encountering the same friction.

## Week 2: ship the quick wins

The 5 quick wins identified in the [prioritisation framework](prioritisation-framework.md) total approximately 5 to 7 days of work. None require major engineering.

- Day 1 to 2: progress indicator and message during first mobile login.
- Day 3: "US only" label on regional cashback promotions.
- Day 4: one-line workspace explanation and auto-default of the newly created workspace.
- Day 5: clear pricing message at sign-up.
- Day 6 to 7: walkthrough audit and screenshot refresh.

Each shipped change should be paired with a measurement plan. We need to know whether the change moved the metric.

## Week 3: listen

- **Run a short survey** of recent non-US sign-ups, focused on the perception of regional relevance and the clarity of the onboarding flow. Goal: understand whether the cashback issue is representative of a broader localisation gap, or an isolated friction point.
- **Sit in on Concierge** for several hours each day during week 3, listening for any of the 5 issues showing up in real conversations.
- **Speak with one engineer and one product manager** about whether the proposed quick wins create downstream complexity I have not considered. (As a Generalist, my job is to carry customer signal toward the team, not to ship without consultation.)

## Week 4: test and report

- **A/B test the workspace setup explanation and the pricing clarity changes** against the previous version. Define success criteria before the test starts: a 5 percent or greater improvement in onboarding completion would justify making the change permanent.
- **Present findings to the team** in a written brief. Include: what we measured, what we shipped, what moved, what did not move, and what I propose for month 2.
- **Pre-write the month 2 plan** as a draft that the team can react to, rather than waiting to be asked.

## Reporting cadence

I would propose a single written update at the end of each week, posted as a comment on a meta-Issue in the relevant repo. Public, async, scannable in 60 seconds. Matches how I understand the team to operate.

## A note on this plan

The plan is deliberately conservative in week 1. The instinct in a new role is to ship quickly to demonstrate impact. The more useful instinct is to confirm the problem before fixing it. Shipping a change against an unvalidated hypothesis can reduce trust in the role over time, even if the individual fix lands well.

The trade-off I am making explicit: 1 week of validation in exchange for higher confidence that weeks 2 to 4 are spent on the right things.

Last updated: 27 April 2026.
