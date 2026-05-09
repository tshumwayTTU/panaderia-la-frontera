# Project Plan

This plan covers the risk strategy and work breakdown for delivering the Panadería La Frontera website by May 8, 2026 at 11:59 PM Central. It applies the planning framework from *Project Management for the Unofficial Project Manager*: identify and TAME risks, break the work down into deliverables, components, and activities, sequence and estimate them, and identify the critical path.

## Risk Strategy

### Risk identification and prioritization

Each risk is scored 1–5 on Impact (severity if it happens) and Probability (likelihood). Risks scoring 12 or higher get an explicit TAME plan. Lower-scoring risks are acknowledged but not formally planned.

| # | Risk | Impact | Probability | Score | Strategy |
|---|---|---|---|---|---|
| 1 | Time slippage past the May 8 deadline | 5 | 1 | 5 | Acknowledged |
| 2 | Retrospective written hollow under time pressure | 4 | 3 | 12 | Mitigate |
| 3 | Scope creep | 5 | 3 | 15 | Mitigate |
| 4 | Image cohesion across product photos | 3 | 4 | 12 | Mitigate |
| 5 | Missing rubric targets across the three sections | 5 | 3 | 15 | Mitigate |
| 6 | Personal time / burnout conflict with other commitments | 3 | 2 | 6 | Acknowledged |

### TAME plans for high-priority risks

**Risk 2: Retrospective hollowness (Mitigate).** I'll keep a running notes file outside the repository to track memorable moments and decisions during the build. When I write the retrospective, those notes feed directly into the three-question structure (what went well, what went wrong, what I'd do differently).

**Risk 3: Scope creep (Mitigate).** The Exclusions list in `scope.md` is the explicit mitigation. I review it before each commit to confirm anything new still fits within scope.

**Risk 4: Image cohesion across product photos (Mitigate).** I reduced photo dependence from four products to two (concha and rosca de reyes); empanadas and pan dulce are represented with CSS-styled cards instead. This eliminates the cohesion problem at the source rather than trying to color-grade four mismatched photos after the fact.

**Risk 5: Missing rubric targets (Mitigate).** The Project 03 rubric has three weighted sections: PM Documentation (50 pts), Technical Implementation (30 pts), and Synthesis & Professionalism (20 pts). Before writing each deliverable, I check the rubric to see what it's asking for. The pre-submission rubric pass (Schedule activity 9) is the final check.

### Acknowledged below the threshold

- **Risk 1: Time slippage past the May 8 deadline.** Score 5 (Impact 5 × Probability 1). The deadline is firm, but probability is low based on my experience as a developer estimating similar work. I've baked the mitigation into the schedule itself: tight durations, daily milestones, and a half-day buffer on May 8.
- **Risk 6: Personal time / burnout conflict.** Score 6 (Impact 3 × Probability 2). Other commitments will compete for time during the build, but I've already baked the work-vs-duration distinction into the schedule's durations, which reflect calendar time around real life rather than pure work hours.

## Work Breakdown Structure

The WBS decomposes the project into deliverables (nouns), then components (sub-deliverables that enable a higher one), then activities (verbs). The activities listed below are the same items sequenced in the Schedule section: the schedule is where these activities get durations, predecessors, and target dates.

- **Planning documents** (deliverable)
  - `scope.md` (component) — revise from Assignment 03 import
  - `plan.md` (component) — draft risk strategy, WBS, schedule, and critical path
  - `retrospective.md` (component) — write three-question reflection per PMUPM Ch. 7
- **Website** (deliverable)
  - `index.html` (component) — build homepage with bakery identity, products, location, and hours
  - `about.html` (component) — build family story page
  - `style.css` (component) — write base styles in a warm palette (terracotta, cream, deep brown)
  - Imagery (component) — integrate two product photos (concha, rosca de reyes) and CSS-styled cards for empanadas and pan dulce
- **Repository and deployment** (deliverable)
  - GitHub repo `panaderia-la-frontera` (component, initialized)
  - `.gitignore` (component, done)
  - GitHub Pages deployment (component) — push to GitHub, enable Pages, verify live URL
  - `README.md` (component) — write README linking to live site and docs
- **Submission** (deliverable)
  - Pre-submission rubric pass (component) — run pre-submission rubric pass against all three rubric sections
  - Canvas submission (component) — submit repository URL on Canvas

## Schedule

Today is May 8, 2026 (Friday). Deadline is tonight at 11:59 PM Central.

Durations below reflect duration (calendar time), not raw work (hours of effort). A two-hour writing task can span half a day because real life happens around project work. Durations are deliberately tight to avoid Parkinson's Law (work expanding to fill the time allotted). The conditional activity 5 (style polish) is the only built-in slack.

All dependencies below are Finish-to-Start (each activity must finish before the next can start): the only dependency type applicable to a strictly sequential solo project.

| # | Activity | Duration | Predecessor | Target |
|---|---|---|---|---|
| 1 | Revise `scope.md` | 0.5 day | — | May 3 (done) |
| 2 | Draft `plan.md` | 0.5 day | 1 | May 5–8 |
| 3 | Build `index.html` + base `style.css` | 0.5 day | 2 | May 8 |
| 4 | Build `about.html` | 0.5 day | 3 | May 8 |
| 5 | Polish styles + run W3C validation (conditional) | 0.5 day | 4 | May 8 |
| 6 | Push to GitHub, enable Pages, verify live URL | 0.25 day | 5 | May 8 |
| 7 | Write `README.md` with the live URL | 0.5 day | 6 | May 8 |
| 8 | Write `retrospective.md` | 0.5 day | 7 | May 8 |
| 9 | Run pre-submission rubric pass | 0.25 day | 8 | May 8 |
| 10 | Submit on Canvas | 0.1 day | 9 | May 8 (well before 11:59 PM) |

### PERT estimate for the highest-uncertainty activity

Most activities above have predictable durations. The exception is activity 3 (build `index.html` + base `style.css`) because design choices (palette tuning, typography pairing, hitting the warm/handmade brief) take more iteration than the HTML and CSS coding itself. PERT formula `(O + 4N + P) / 6`:

- Optimistic (O): 0.25 day — design lands first try, no iteration
- Normal (N): 0.5 day
- Pessimistic (P): 1 day — multiple design iterations on palette or layout

PERT estimate: (0.25 + 4×0.5 + 1) / 6 ≈ **0.5 days**.

## People Resources

Solo project. I own every activity above. Outside inputs are two peer reviewers (Assignment 04, complete) and the instructor (final grading). This plan is how I communicate the risk strategy and schedule to the instructor.

## Critical Path

Because this is a solo project with strictly sequential deliverables (each commit depends on the prior one), the critical path runs through every activity in the schedule above. There's no parallel work to fall back on, so any slip pushes the whole project.

## Milestones

Decision points where I stop, verify direction, and confirm readiness to proceed:

- **M1 — Scope finalized (May 5):** Confirm peer-confirmed elements are preserved and self-review refinements are applied. Triggers start of `plan.md`.
- **M2 — Plan finalized (May 8):** Confirm risks and schedule still align with May 8. Triggers start of build.
- **M3 — Site code complete (May 8):** Confirm W3C validation passes and the 375px viewport check holds. Triggers deploy.
- **M4 — Site deployed (May 8):** Confirm the live URL renders both pages correctly. Triggers `README.md`.
- **M5 — All docs complete (May 8):** Confirm rubric coverage across `scope.md`, `plan.md`, and `retrospective.md`. Triggers pre-submission pass.
- **M6 — Pre-submission rubric pass (May 8):** Final go/no-go before Canvas submission.

## Plan flexibility

Plans like this work in rolling waves: as the project unfolds and information becomes more reliable, the plan adapts. This is the May 8 wave; I've already adapted it once (I mitigated the image cohesion risk during planning by reducing photo dependence to two products) and may adapt it again as build-phase realities surface.
