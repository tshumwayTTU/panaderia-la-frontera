# Project 03 Retrospective

A reflection on the Panadería La Frontera build, answering the three key retrospective questions from PMUPM Ch. 7. Project scope fulfillment and final sign-off come through instructor grading, so this retrospective focuses on the reflection itself.

## What went well

The planning documents earned their weight. Scope and plan together made up half the rubric, and front-loading them meant the build had clear targets to hit instead of inventing decisions in real time. The exclusions list especially: every "should I add..." impulse during the build had a one-line answer in `scope.md`.

Catching the image cohesion problem at planning time saved real build hours. Risk 4 in `plan.md` identified that four free stock photos from four different photographers wouldn't cohere visually. Reducing photo dependence to two products (concha and rosca de reyes) and using CSS-styled cards for the other two prevented a multi-hour color-grading rabbit hole during the build phase.

Commits mapped cleanly to WBS deliverables. The git log reads as a project arc rather than a stream of changes, which made it easy to see what was done and what was left at any moment during the deadline-day push.

Self-review filled the gap when peer feedback didn't include specific suggestions for change. Both Assignment 04 reviewers responded positively, and treating that as a signal to do a structured self-review surfaced three real refinements: an explicit repo URL and live site link in the scope's description, an updated rubric target reflecting Project 03's three-section structure (the original referenced Assignment 03's tier language), and a sharper responsive boundary at 375px instead of "reasonable responsive behavior."

## What went wrong

The build started four days late. The plan scheduled the build to start May 4, one day after the scope was revised. It actually started May 8, the deadline day. Two days of buffer evaporated, and the conditional style-polish commit had to be cut just to ship on time.

The first risk list had filler. Items like "W3C validation failing," "browser quirks at small viewports," and "GitHub Pages deploy fails on first push" were really just build requirements wearing risk costumes. Each is a step you have to complete, not something that might go wrong. Trimming the list took two or three review rounds before the risks left were genuine.

The peer-review feedback loop didn't produce specific critique. Both Assignment 04 reviewers gave positive responses without recommendations for change, which left self-review carrying the revision burden.

## What I'd do differently

Treat schedule start dates as commitments, not forecasts. The plan's buffer is for genuine schedule risk like illness or competing priorities, not for absorbing procrastination on the build phase. Putting the build on the calendar as a commitment to myself would have prevented this project's biggest miss.

Apply a sharper risk filter during plan brainstorming. The deeper test is whether I have a real choice in how to respond, or just have to fix it. Build requirements fail that test and shouldn't appear on the risk list.

Seek reviewers from friends or family who can give specific, actionable critique on the next project. Bringing in someone I know to "find one thing that could be tighter" would produce substantive input that complements assigned peer review.
