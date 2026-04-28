# 03. Workspace Setup Lacks Clarity

| Field | Value |
|---|---|
| Priority | High |
| Area | Onboarding, Product Clarity |
| Effort | Quick win (1 to 2 days), plus medium-term flow differentiation |
| Status | Proposed |

## Problem

During onboarding, I was prompted to create a workspace without a clear explanation of why it was necessary or what operational purpose it served. After creation, the new workspace did not automatically become the default, requiring an extra step that felt unnecessary.

This created hesitation during onboarding and slowed initial product adoption.

## Customer impact

When users do not understand why they are completing a setup step, friction increases. Every moment of confusion during onboarding is a moment where the user questions whether the product is right for them.

For individual users (rather than enterprise admins), the concept of "workspaces" may feel unnecessarily complex. The mental model of "I just want to track my expenses" does not map cleanly to "first, create a container to track them in."

## Evidence

Direct observation during testing in April 2025. During onboarding the workspace creation step appeared with minimal explanation. After creation, the newly-created workspace was not auto-selected as the default. (Figure: see [original-submission/](../original-submission/), Fig. 2.)

## Hypothesis on cause

Two hypotheses, neither mutually exclusive:

1. The workspace concept is essential for the team and enterprise products, so it was kept in the individual flow for consistency and to avoid divergent codepaths.
2. The auto-default behaviour was an oversight, or was intentionally avoided to give users explicit control, but at the cost of an avoidable extra step.

Either way, the symptom is the same: an individual user encounters complexity that does not serve them.

## Proposed solutions

**Quick win (1 to 2 days):** add a one-line explanation during workspace setup. Suggested copy: "Workspaces help organise expenses by team, department, or business entity. You can always change this later." Also auto-set the newly created workspace as the default.

**Medium-term (1 to 2 months):** create differentiated onboarding flows. Individual users skip workspace setup entirely (system auto-creates a default workspace). Team and enterprise users get the full workspace configuration step. This reduces friction for the majority of new sign-ups while preserving the existing flow for users who actually need it.

**Strategic (longer-term):** evaluate whether the workspace concept itself can be re-named for individual users. The word "workspace" is doing two jobs: a data container and a permissions boundary. For an individual user, that distinction is irrelevant.

## Expected outcome and validation

If 30 percent of new users hesitate at this step (illustrative), and 5 percent abandon onboarding because of it, that is a measurable conversion loss. With an illustrative 50,000 new sign-ups per month, that would be approximately 750 users lost at a step that could be made clearer with one tooltip.

Both percentages and the user-volume figure are illustrative.

Validation plan:

1. Pull telemetry on time-to-progress at the workspace creation step.
2. Identify drop-off rate at this specific step.
3. Pull Concierge tickets containing the term "workspace" and assess what proportion are individual users asking what a workspace is.
4. After shipping the quick-win tooltip, measure time-to-progress and abandonment rate change at this step.
5. After shipping the differentiated flow, compare onboarding completion rates between individual and team paths.

## Open questions

- What is the current breakdown of new sign-ups by intent (individual, team, enterprise)?
- Has the team previously considered hiding workspace setup from individual users, and if so, what was the reason for keeping it?
- What downstream features assume the user has explicitly named their workspace (rather than it being auto-created)?
- Are there compliance or audit reasons workspaces must be explicitly created rather than auto-defaulted?

## Linked resources

- [Issue #3](../../../issues/3)
- [Original screenshot evidence](../assets/screenshots/) (figure to be added)
- [Prioritisation framework](../docs/prioritisation-framework.md)

Last updated: 27 April 2026.
