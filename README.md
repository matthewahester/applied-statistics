# applied-statistics

Public-facing Quarto **course-materials site** for **Applied Statistical Methods**, assembled
by Matt Hester. Sibling to the main site
[matthewhester.com](https://matthewhester.com); intended to live at
`/applied-statistics/` under that domain.

This is **assembled course material** — synthesized lesson notes,
hands-on R labs, and curated references for choosing, running, interpreting, and communicating common applied analyses. It is a durable
public resource site, **not** a record of a currently scheduled section,
and **not** an LMS.

## Status

Assembled from a course-material build (2026-06); a coherent **draft**,
not a finished release. Topic flow, notes, labs, and resources are in
place. Example datasets are synthetic and the numbers are provisional;
dates, weights, and final policies are not sealed and are authoritative
in the LMS (Blackboard) whenever the course runs.

## What this site holds

- **Notes** — the weekly instructional spine (15 weeks, four parts): statistical questions and data structure, exploratory and graphical comparison, estimation and uncertainty, one-sample/paired and two-group comparisons, one-way and two-way ANOVA with interaction, assumptions and diagnostics, multiple comparisons, regression review, ANCOVA and adjustment, contingency tables, and logistic regression for binary outcomes.
- **Labs** — four hands-on R labs (two-group comparison and effect size, ANOVA with multiple comparisons, building and checking a regression, logistic regression and odds ratios).
- **Resources** — a methods glossary, a method-chooser decision guide, an assumptions-and-diagnostics guide, and a reporting-and-interpretation guide.

The notes are the course's **own synthesis**. R code is shown as
**static, non-executed** ```r fences (worked numbers are hand-authored
synthetic listings with seeds set); no R engine is invoked, so the site
renders deterministically.

## What does not go in this repo

Anything private to a graded offering: answer keys, assessment items,
rubrics, point values, due dates, student data, or any directory from the
private course build (`_state/`, `assessment_shadow/`, `source_text/`,
`run_reports/`, `accessibility/`). See [`CLAUDE.md`](CLAUDE.md) for the
full list. The operational, graded side of any live offering lives in
**Blackboard (the LMS)**, which is authoritative.

## Local development

```bash
quarto render     # build to _site/
quarto preview    # live preview
```

R code is shown as **static, non-executed** ```r fences, so the site
renders **fully with plain `quarto render` — no R required**.

No CI and no deploy pipeline in this repo. The combined site is assembled
and deployed by the hub repo (`matthewhester-site`). Local builds only
here; commits are deliberate and user-driven.
