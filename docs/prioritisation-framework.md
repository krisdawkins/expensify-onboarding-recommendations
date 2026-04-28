# Prioritisation Framework

How the 5 issues were scored, ranked, and bucketed. Includes the cumulative impact model.

## Scoring

Each issue was scored on three dimensions on a 1 to 5 scale, where higher means more urgent.

- **Customer impact (1 to 5):** how much the issue costs in trust, time, or progress.
- **Frequency (1 to 5):** how often a user in this persona would encounter it.
- **Effort to fix (1 to 5):** inverted scale, where 5 means a same-day copy or config change and 1 means strategic, multi-quarter engineering work.

| Issue | Customer impact | Frequency | Effort to fix | Priority |
|---|---|---|---|---|
| Slow mobile loading on first login | 5 | 5 | 4 | Highest |
| Cashback messaging: regional bias | 4 | 5 | 2 | Highest |
| Workspace setup lacks clarity | 3 | 5 | 2 | High |
| Free trial pricing unclear | 4 | 3 | 1 | High |
| Inbox walkthrough mismatch | 2 | 3 | 1 | Medium |

## Why these three dimensions

Customer impact alone overweights edge cases that hurt a few users badly. Frequency alone overweights cosmetic issues seen by everyone. Effort alone biases toward easy wins regardless of value. Combining all three gives a balanced picture of where to start.

The three-dimension model is a working tool, not a finished science. In a real role I would calibrate the scores against actual analytics rather than a single tester's judgement.

## Cumulative impact model

Each friction point compounds the next. A user who waits 3 minutes to log in, then sees irrelevant US promotions, then does not understand workspaces, then is confused about pricing, has experienced four trust-eroding moments before submitting a single expense.

The estimates below are illustrative, intended to show the shape of impact rather than predict precise figures.

| Step | Friction | Estimated drop-off | Cumulative retention |
|---|---|---|---|
| First mobile login | 3-minute delay, no feedback | ~10% | 90% |
| Dashboard / promotions | Irrelevant US cashback messaging | ~3% | 87% |
| Workspace setup | Unclear purpose, not auto-defaulted | ~5% | 83% |
| Pricing / trial | Confusion about future costs | ~3% | 80% |
| Inbox walkthrough | Instructions do not match the UI | ~1% | 79% |

Estimated outcome: approximately 1 in 5 new users may be lost during onboarding due to cumulative friction, before they have experienced any core product value.

Fixing the top three issues alone could improve onboarding completion by 15 to 18 percent on these assumptions.

## A note on the numbers

The drop-off percentages above are directional estimates, not measured rates. They were generated to illustrate compounding effects, not to predict revenue.

The first action in the [30-day plan](30-day-plan.md) is to validate this model against actual product analytics. If real drop-off rates are smaller, the prioritisation may shift. If they are larger, the urgency increases. Either way, this framework is the starting point for that conversation, not the conclusion of it.

## Quick wins summary

| Issue | Quick win | Effort | Impact |
|---|---|---|---|
| Slow first login | Add progress indicator and contextual message | 1 day | High |
| Cashback regional bias | Add "US only" label to promotions | 1 day | High |
| Workspace confusion | Add one-line explanation and auto-default the workspace | 1 to 2 days | Medium-high |
| Pricing unclear | Add a clear pricing line at sign-up | 1 day | Medium |
| Walkthrough mismatch | Audit and update walkthrough screenshots | 1 to 2 days | Low-medium |

Total effort for all five quick wins: approximately 5 to 7 days. No major engineering required. All are copy, configuration, or documentation changes.

Last updated: 27 April 2026.
