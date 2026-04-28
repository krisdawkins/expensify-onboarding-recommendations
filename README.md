# Expensify Onboarding Recommendations

Onboarding research and 5 prioritised recommendations for Expensify, written as part of the Customer Experience Generalist UK final round.

## Executive summary

I tested Expensify on web (Chrome, macOS) and mobile (iOS) for approximately 2 hours across two sessions in April 2025, focused on the onboarding journey and first-use experience for a first-time UK-based individual user.

I identified 5 friction points, four of which occur in the first 10 minutes of use. The connecting theme is that the onboarding experience is optimised for US-based power users, not international first-time users. Together these create a compounding trust deficit during the most fragile window of the user journey.

If the top three issues are addressed with the proposed quick wins, my view is that onboarding completion would meaningfully improve, particularly for non-US first-time users. The quick wins total under two weeks of work and require no major engineering, only copy, configuration, and documentation changes.

## Top 3 recommendations at a glance

| Issue | Priority | Quick win | Effort |
|---|---|---|---|
| [Slow mobile loading on first login](recommendations/01-mobile-load-time.md) | Highest | Add a progress indicator with contextual messaging | 1 day |
| [Cashback messaging shows US-only benefits to non-US users](recommendations/02-cashback-us-only.md) | Highest | Add a "US only" label on regional promotions | 1 day |
| [Workspace setup lacks clarity for individuals](recommendations/03-workspace-setup.md) | High | Add a one-line tooltip and auto-default the workspace | 1 to 2 days |

The remaining two recommendations are in the [recommendations folder](recommendations/).

## How to read this repo

- Start here, the [README](README.md), for the executive summary.
- For the full per-issue analysis, see the [recommendations](recommendations/) folder. Each file follows the same 8-section structure.
- For methodology, see [docs/methodology.md](docs/methodology.md).
- For the prioritisation framework and the cumulative impact model, see [docs/prioritisation-framework.md](docs/prioritisation-framework.md).
- For what I would do in the role across the first 30 days, see [docs/30-day-plan.md](docs/30-day-plan.md).
- For how AI was used in producing this work, see [docs/ai-reflection.md](docs/ai-reflection.md).
- For the limitations of this analysis, see [docs/limitations.md](docs/limitations.md).
- The 5 recommendations are also tracked as [Issues](../../issues), each linked to its full markdown file.

## Methodology in two lines

Persona: first-time UK-based individual user setting up Expensify for personal expense tracking. Surface tested: web (Chrome, macOS) and mobile (iOS). Duration: approximately 2 hours across two sessions, April 2025.

## Limitations

This analysis is based on a single tester, a single persona, and approximately 2 hours of hands-on use. The business impact estimates throughout this repo are illustrative, intended to show the shape of impact rather than predict precise figures. Validating those estimates against actual product analytics would be the first action in the [30-day plan](docs/30-day-plan.md). See [docs/limitations.md](docs/limitations.md) for a fuller statement.

## About this work

Prepared by Kristofer Dawkins as part of the Expensify Customer Experience Generalist UK process. Originally submitted as a PDF in April 2025 and restructured into this repository in April 2026 ahead of the final round, with the original PDF archived in [original-submission](original-submission/).

This repository is open to feedback. See [CONTRIBUTING.md](CONTRIBUTING.md).

Last updated: 27 April 2026.
