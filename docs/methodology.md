# Methodology

How this research was conducted. Brief, because a long methodology section on a 2-hour test would be dishonest.

## Persona

**First-time UK-based individual user setting up Expensify for personal expense tracking.**

Why this persona:

- I had used Concur extensively in previous roles, so I came to Expensify with a working benchmark for what an expense management tool should feel like, but no prior exposure to the Expensify product itself.
- The UK lens is deliberate. Expensify is US-headquartered, and one of my hypotheses going in was that international first-time users would experience friction that US users have learned to ignore.
- Individual rather than enterprise admin, because individual users are the ones most likely to abandon onboarding silently. Enterprise admins typically have a mandate to push through friction.

This persona is one slice. The recommendations should be tested against other personas (admin, finance lead, ops manager, multi-country team) before commitment. See [limitations](limitations.md).

## Surface tested

- **Web:** Chrome on macOS.
- **Mobile:** iOS.
- Both interfaces, in sequence, simulating a real first-time user creating an account on web and continuing on mobile.

## Duration

Approximately 2 hours across two sessions in April 2025.

## Focus

The onboarding journey, first-use experience, and early-adoption friction points. I deliberately did not test:

- Admin configuration of policies, categories, tags, and approvals.
- Integration setup beyond the auth screen (QuickBooks, Xero, NetSuite).
- The Expensify Card transaction flow (no card to test with).
- Concierge support across multiple ticket types (only the surface look-and-feel).
- Expensify Travel.

Anything in those areas is outside the scope of this analysis.

## What I did

1. Created an account on the web platform.
2. Walked the onboarding flow as instructed.
3. Created a workspace.
4. Submitted a manual expense and a SmartScanned receipt.
5. Submitted a report.
6. Connected an integration (auth screen only).
7. Opened the Concierge chat.
8. Skimmed in-app help.
9. Logged into the mobile app for the first time, immediately after web setup.
10. Walked the same flows on mobile.

I took notes in real time and screenshot every friction point.

## How I prioritised

Each issue was scored on three dimensions on a 1 to 5 scale:

- **Customer impact:** how much trust or progress the issue costs the user.
- **Frequency:** how often this would be encountered by users in this persona.
- **Effort to fix:** inverted (5 = quick fix, 1 = strategic engineering).

Priority bands: Highest, High, Medium. See [prioritisation-framework.md](prioritisation-framework.md) for the full table and the cumulative impact model.

## How AI was used

AI was used as a thinking partner for industry benchmarks, framework pressure-testing, and editorial polish. All observations and prioritisation decisions are mine, based on direct use of the product. See [ai-reflection.md](ai-reflection.md) for the full statement.

Last updated: 27 April 2026.
