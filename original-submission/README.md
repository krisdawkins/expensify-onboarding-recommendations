# Original Submission Archive

This folder is the archive of the original Round 2 PDF submission, kept here for transparency and traceability.

## What lives here

- The original PDF (to be added when uploaded to GitHub).
- The original screenshots referenced as Fig. 1 through Fig. 4 in the recommendations (to be added).
- This README, explaining the relationship between the original submission and the rest of the repository.

## Why keep the original

Three reasons.

First, it shows the work as it was actually delivered for Round 2, without rewriting history. Anyone reviewing the repo can see the starting point and the evolution.

Second, it preserves the screenshot evidence in one place, so the recommendation files can reference figures by number rather than embedding large images inline.

Third, it makes the diff visible. The recommendations in the [recommendations/](../recommendations/) folder are not a copy of the PDF. They are a translation: same content, restructured for GitHub, with explicit hypotheses, validation plans, and open questions added. Keeping the original alongside the translation makes that work visible.

## What changed in the translation

The PDF presented five recommendations as a single linear document. The repo presents them as:

- One README at the root with the executive summary and top-three table.
- Five separate recommendation files, each with a consistent eight-section structure (problem, customer impact, evidence, hypothesis on cause, proposed solutions, expected outcome and validation, open questions, linked resources).
- Five supporting documents in [docs/](../docs/) covering methodology, prioritisation, the 30-day plan, AI reflection, and limitations.
- A [CONTRIBUTING.md](../CONTRIBUTING.md) at the root that sets the tone for feedback.

Content carried over without changes:

- The five recommendations themselves (mobile load, cashback, workspace, pricing, walkthrough).
- The prioritisation framework (impact, frequency, effort).
- The cumulative impact model and the illustrative-numbers caveat.
- The 30-day plan.
- The AI reflection.

Content added in the translation:

- An explicit hypothesis-on-cause for each recommendation, separate from the proposed fix.
- A validation plan for each recommendation, listing the specific data sources to pull.
- Open questions for each recommendation, surfacing what I would want to learn from the team.
- A standalone [limitations.md](../docs/limitations.md) consolidating every assumption and caveat.

Nothing was removed. The translation is additive.

## How to read this

If you want the original work as submitted, read the PDF in this folder.

If you want the same content restructured for navigation, prioritisation, and follow-up, start at the [root README](../README.md) and follow the links.

Both versions reflect the same two hours of testing on the same persona, in April 2025.

Last updated: 27 April 2026.
