# 01. Slow Mobile App Loading During First Login

| Field | Value |
|---|---|
| Priority | Highest |
| Area | Performance, Onboarding |
| Effort | Quick win (1 day), plus medium-term and strategic work |
| Status | Proposed |

## Problem

After successfully creating my account on the web platform, the mobile app took approximately 3 minutes to load on first-time login. During that time the screen showed no progress indicator, no loading message, and no other feedback. Just a solid white screen.

This created uncertainty about whether the setup had worked, the password was correct, or the app was malfunctioning.

## Customer impact

First login is the single most fragile moment in onboarding. The user has invested attention to set up an account and is asking, in effect, "did this work?" A 3-minute silent wait at that moment provides the wrong answer.

In the persona of a first-time UK-based individual user, this is the moment where trust is built or broken.

## Evidence

Direct observation during the testing window in April 2025. Specifically:

- Account created on web, immediately followed by mobile install.
- Mobile login attempted with the same credentials.
- App displayed a white screen for approximately 3 minutes after authentication.
- No spinner, no message, no progress indicator.
- After 3 minutes the home view loaded normally.

I did not test alternative network conditions, alternative regions, or repeat first-logins (the issue is by definition a first-login phenomenon).

## Hypothesis on cause

The most likely candidates, in rough order of probability:

1. Initial workspace data sync after first authentication, blocking the UI thread.
2. Asset download (images, JS bundles) on first load, with no cached version available.
3. API call latency for one or more authentication or session-establishment endpoints.
4. A combination of the above, where each adds a few seconds and the compound effect is the 3-minute wait.

Without backend logs and a profiled mobile session, this is inference, not diagnosis. The first action below is to confirm the cause.

## Proposed solutions

**Quick win (1 day):** add a progress indicator and a contextual message during first-login load. Suggested copy: "Setting up your workspace. This may take a moment on first login." Minimal engineering effort. Significantly reduces perceived wait time and the doubt-of-app-working failure mode.

**Medium-term (1 to 3 weeks):** profile the mobile app's first-login flow to identify the cause of the delay. Optimise the most expensive step (sync, asset download, or API). Target: first login under 10 seconds end-to-end.

**Strategic (1 to 2 quarters):** implement progressive loading. Show the core interface immediately and load secondary features in the background. Industry benchmark: most well-engineered consumer mobile apps load to a usable interface within 3 to 5 seconds on first login.

## Expected outcome and validation

If even 10 percent of new mobile users abandon during this delay, with an illustrative onboarding rate of 50,000 users per month, that is approximately 5,000 potential customers lost at the first touchpoint, before Expensify has had the opportunity to provide any product value on its mobile app.

Both the 10 percent figure and the 50,000 figure are illustrative. The validation plan, in order:

1. Pull mobile first-login latency analytics from existing telemetry.
2. Cross-reference with first-session abandonment rates.
3. Replace the illustrative numbers above with real numbers.
4. After shipping the quick win, measure perceived-wait improvement via user testing or post-onboarding survey.
5. Measure abandonment rate change before and after the medium-term optimisation.

Industry reference: Google's research on mobile page load times indicates that 53 percent of mobile users abandon pages that take longer than 3 seconds to load. This is a directional reference, not a precise prediction of Expensify's situation.

## Open questions

- What does first-login latency look like across regions and network types?
- Is the 3-minute observation reproducible across other test devices, or specific to my hardware?
- What is the current first-session abandonment rate, and how does it correlate with measured first-login latency?
- Is there an existing telemetry pipeline measuring first-login load time, or would this need to be instrumented?

## Linked resources

- [Issue #1](../../../issues/1) (in the Issues tab of this repo)
- [Original screenshot evidence](../assets/screenshots/) (figure to be added)
- [Prioritisation framework](../docs/prioritisation-framework.md)

Last updated: 27 April 2026.
