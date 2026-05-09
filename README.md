# Panadería La Frontera

A two-page static website for a fictional family Mexican-American bakery in El Paso: three generations of pan dulce, hand-scored at 4 AM.

**Live site:** [tshumwayttu.github.io/panaderia-la-frontera](https://tshumwayttu.github.io/panaderia-la-frontera)

## What this is

This is a portfolio project for Project 03 of an academic class on project management and web development. The brief was to build and deploy a real static website while applying the planning principles from *Project Management for the Unofficial Project Manager* (PMUPM) and the generalist mindset from *Range*. The bakery is fictional. The PM workflow, the build, and the design choices are real.

## Design intent

The scope called for a warm, handmade, third-generation feel. The concha photo sets the mood on the homepage. The two-page constraint forces every section to do real work, and the about page uses a heading-left layout so the family story can run long.

## The site

- **[Home](https://tshumwayttu.github.io/panaderia-la-frontera/)**: bakery identity, four core products, location, hours, contact
- **[Our Story](https://tshumwayttu.github.io/panaderia-la-frontera/about.html)**: three-generation family narrative

## How it's built

Plain HTML5 and CSS3 with semantic markup. A single stylesheet (`style.css`) drives both pages. Imagery comes from Pexels under their free license. Headings use Playfair Display via Google Fonts. Body type is the system sans stack.

## Project management documentation

I scoped, planned, and reflected on this build using the PMUPM framework. Each doc in `docs/` is committed alongside the code it shaped:

- **[scope.md](docs/scope.md)**: project scope statement: purpose, deliverables, exclusions, priorities, acceptance criteria (PMUPM Ch. 3)
- **[plan.md](docs/plan.md)**: risk strategy with TAME plans, work breakdown structure, schedule with PERT estimate, critical path, milestones (PMUPM Ch. 4)
- **[retrospective.md](docs/retrospective.md)**: three-question reflection: what went well, what went wrong, what I'd do differently (PMUPM Ch. 7)

## Where the PM informed the build

A few specific places where the planning documents shaped the actual code:

- **The scope's exclusions list**: Ruled out JavaScript, frameworks, real-business claims, and extra pages. I re-read it before every commit to mitigate scope creep.
- **The plan's image cohesion risk**: Drove the decision to use only two photos (concha, rosca de reyes) and represent the other two products with CSS-styled cards rather than force four mismatched photos to look unified.
- **The plan's WBS and critical path**: Mapped commits to specific deliverables, so the git history reads as a project timeline.

## Credits

- Concha photo: [Miguel Rodriguez](https://www.pexels.com/@miguel-rodriguez-1844391833/) via Pexels
- Rosca de Reyes photo: [Erick Ortega](https://www.pexels.com/@erickfoto/) via Pexels
- Typography: Playfair Display via [Google Fonts](https://fonts.google.com/)
- PM framework: Kogon, K., & Blakemore, S. (2024). *Project management for the unofficial project manager* (Updated and rev. ed.). BenBella Books.

## Disclaimer

Panadería La Frontera is a fictional bakery created for an academic project. No real business is implied. The contact information shown on the site is not real.
