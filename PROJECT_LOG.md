# Learn.it — Project Log

A running record of what has been done and what's planned. Newest entries at the top of each section. Update this file whenever work lands.

## Done

### 2026-10-07 — Light theme by default (`274d9e6`)
- Site no longer follows the OS dark mode. Light is the default; dark only when chosen with the toggle (saved in `localStorage['ledger-theme']`).

### 2026-10-07 — Team pass: track switcher, motion, AI track, verified resources (`c78431d`)
- Top-bar **Java Developer / AI Engineer** switcher on every page (phones get a full-width row). Switches in place on Home/Practice/Projects, navigates on Roadmap/Topic. Per-track accent: green (Java), indigo (AI).
- New landing page with animated track backgrounds (class graph for Java, neural net for AI).
- Motion components in `components/motion/` (page enter, reveals, count-ups, spring progress bars, collapsible topic steps, "you are here" marker, scroll spine). All respect reduced motion.
- Fixed: pages invisible under OS "reduce motion"; quiz answer always being option 1 (now a deterministic shuffle).
- AI track: 6 roadmap sections, 6 Practice subjects, projects grouped by section, 14 content fixes. Readiness gates stay Java-only.
- Resources: all 260 LeetCode links verified; 19 broken/weak links replaced; all 67 Algorithm List links now direct pages; validator rejects search URLs.
- One consistent nav + page header; ~420 lines of dead CSS removed.

### 2026-09-23 — UX redesign: "show only what's needed now" (`2d59022`)
- Home = one Continue Learning action. Roadmap = one row per topic, grouped by tier. Topic = stepper (one subtopic open at a time). New Practice and Projects pages. 4-item nav.

### 2026-09-23 — Editorial "Field Notes" design (`b2714fd`)
- Fraunces serif, warm paper palette, hairline rules.

### 2026-09-23 — Curriculum fixes and content-quality audit (`fbbe4db`)
- `java-fundamentals` remainder renamed to `core-java` (prevented false progress); Kubernetes made optional; 26 numbered phases; named readiness gates; quiz/mini-project/subtitle fixes from a full content audit.

### 2026-09-23 — Java curriculum refinement (`df335fb`)
- 37 topics / 26 phases, DSA as a parallel track, tier-grouped roadmap.

### Earlier
- `c025e7e` Reliability/security hardening, optimistic locking on progress writes.
- `7c7e7da` Dual-track (Java + AI) guided learning platform.

## Rules that must not break
- Progress keys are `topicId::subtopicIndex::questionIndex` (plus `::concept::`, `::quiz::`, `::project`, `::phaseProject::`). Never rename topic ids or reorder/insert/remove subtopics, questions, checklist items, quiz questions, phases or phase projects — edit text in place only.
- Run `npm run validate`, `npm run build`, and `npm run test:concurrency` before pushing.

## Planned / open
- (Nothing open right now. Add new items here as they come up.)
