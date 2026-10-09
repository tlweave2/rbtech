# riverbanktc.com redesign brief

## Context
- In September 2026 the Riverbank City Council unanimously passed a 45-day data center moratorium, running to about Oct 13. Council said it would revisit the issue at its first October meeting. ([Registry SF](https://news.theregistrysf.com/riverbank-freezes-data-center-rush-with-45-day-moratorium-as-aemetis-pitches-clean-energy-project-on-former-army-munitions-site/), [Oakdale Leader](https://www.oakdaleleader.com/news/public-safety-business-talk-fill-riverbank-agenda/))
- So the people reading this site are skeptical residents and council members, not investors. The site should answer their worries fast, show its evidence, and point to the public process.

## What peer sites do well
| Pattern | Seen at | Used here |
|---|---|---|
| Commitments organized by theme, each with an accountability mechanism | Microsoft Datacenter Community Pledge | 7 commitments, each with "We promise" + "How to check" |
| Plain-language water numbers put in context | Meta (Kuna), Crusoe, Inver Grove Heights applicant | Closed-loop diagram plus "a few homes' annual use" |
| Decibel figures explained in everyday terms | Port Washington, WI city FAQ | FAQ entry on noise (add real dB figure, see TODO) |
| Q&A grouped by category, answering questions residents actually asked | San Angelo, TX city page | FAQ accordion + "ask us, we'll add it" |
| Numeric guardrails (setback, dB at the property line) | Cleveland, TN (Project River) | 200 ft setback diagram; dB still needed |
| Named local partners and community investment | Meta (Kuna) | "Rooted in Riverbank" photo grid |

## Problems with the current site, and the fixes
1. **The opening is a mission statement, not answers.** Fix: the hero says what RTC is in one sentence, followed by four "questions neighbors ask first" cards (water, bills, noise, benefits).
2. **No mention of the moratorium or the public process.** Fix: a status bar plus a "Where things stand" timeline. Saying nothing reads as evasive.
3. **Commitments are only titles.** Fix: each one now has a concrete promise and a way to verify it.
4. **"Not a mega data center" is asserted but never shown.** Fix: a side-by-side comparison table.
5. **No FAQ.** Fix: 9-question accordion, including the moratorium question.
6. **No visuals.** Fix: site diagram (setback), cooling-loop diagram, and real photo slots.
7. **Repetition.** The water and power claims appear 3–4 times in slightly different wording. Fix: one canonical section that the other sections link to.

## Copy inconsistencies to resolve before launch
- **Water amount.** The current site says the fill equals "a few homes' annual needs" in one place and "two homes" in another. Press quotes Spartan saying "an Olympic-size swimming pool." That's about 660,000 gal, which is closer to 5+ homes. Pick one verified gallon figure and use it everywhere.
- **"Zero continuous water usage."** Closed loops still lose some water to leaks and maintenance. State the expected annual top-up honestly.
- **Noise.** "Below the levels allowed" needs an actual dB number at the property line, plus the applicable limit.
- **"Can supply excess power back to the grid"** conflicts with "no on-site power running." Clarify what this means or drop it.
- **$10M+/yr tax and "hundreds" of jobs.** Give the assumptions (assessed value, tax rate, permanent headcount). Unsourced numbers get challenged at council.
- **"First Sustainable Computing Facility in the US"** is a self-defined term. Fine to keep, but define it (the FAQ now does).
- **Capacity (MW) isn't stated anywhere.** Trackers already list 60 MW, so it's better to say it yourselves.

## Assets needed
- The real site plan

- The commitments PDF at `assets/RTC-Responsible-Development-Commitments.pdf`
- Dates for council meetings and community open houses (for the timeline)

## Visual direction
Drawn from the site itself: the 1940s sawtooth-roof plant buildings, technical-drawing linework, and safety-yellow floor-marking accents. Condensed industrial display type (Big Shoulders), Public Sans for body text, and IBM Plex Mono for labels and units. Content sits in ruled ledgers, the way a spec sheet lays it out, instead of a grid of cards. The hero is a cutaway drawing of the building showing the racks, the closed loop, the chillers, the well, and the 200 ft setback.

## Files
- `index.html`: preview hub that links to all three directions
- `previews/a-civic/`: calm civic direction (Fraunces + Inter, teal and sand)
- `previews/b-industrial/`: industrial spec-sheet direction (described above)
- `previews/c-hometown/`: warm, photo-led hometown direction (DM Serif Display + DM Sans, olive and sunset orange)
- `img/`: optimized photos shared by all previews
- No build step. Every page is static HTML.
