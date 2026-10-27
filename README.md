# Algebra pattern guide

A single-page study guide built from worked problem sheets. For each sheet it
records the *pattern* behind the problems — the visual cue that tells you which
method applies — alongside every problem solved step by step.

**Live site:** https://wm.github.io/algebra-two/

## Contents

The page has three topics, switched at the top:

- **Equations** — clearing denominators, distributing awkward coefficients,
  rational equations, substitution, infinite continued fractions, quadratics.
  Built from *Unit 0A 05* and *0A 06 Quiz Review 2*.
- **Lines** — slope, the three forms of a line, perpendiculars, midpoint,
  partitioning a segment by a ratio, distance, and distance from a point to a
  line, intercepts, intersections, and solving for an unknown coordinate or
  coefficient. Built from *0B Homework 1*, *Distance from a point to a line*,
  *Graphing Lines Review 2*, *The Basics of Unit 0B*, the
  *Unit 0B 10-Problem Review*, the *Coordinate Geometry Re-Take* problems,
  problems 1–4 of *Factoring Techniques 05*, and the coordinate geometry
  problem from *The Real Deal 04*.
- **Factoring** — GCF (including a negative GCF), trinomials, the AC method,
  perfect square trinomials (and filling in a missing term), difference of
  squares, sum and difference of cubes, quadratics in disguise, grouping,
  grouping with a special pair, and force-factoring. Built from
  *30 Problem Factoring 02*, *30 Problem Factoring 03*,
  *Factoring Techniques: The Real Deal 01*, *02* and *04*, and problems 5–10
  of *Factoring Techniques 05*.

Each topic has three tabs: a decision **Checklist**, the **Patterns** with their
cues, and the **Solved problems** with collapsible solutions.

The Factoring patterns end with **How the patterns stack**: the multi-step
chains the harder sheets use, plus how to choose which terms to pair, which sign
to pull out, and when a factor is finished. Factoring also has a **Practice
test** tab: seventeen new problems modelled on the Real Deal sheets, with no
hints or labels, each solution naming the solved problem it matches. These were
written for the guide and are not from the teacher.

The Lines topic has a fourth tab, **Practice test**: ten new problems modelled
on the 10-Problem Review, with different numbers and in a different order, plus
an eleventh on a part-to-whole segment ratio (`AQ:AB`). Each has a hidden worked
solution. These were written for the guide and are not
from the teacher.

A fifth tab, **Re-take**, works the seven *Coordinate Geometry Re-Take*
problems in the teacher's style, each linked to the solved problem of the same
type.

## Notes on the answers

Every solution was worked by hand and then verified symbolically with SymPy.
Six answers disagree with the teacher's keys, and each is flagged inline on the
problem itself:

- **0A 05 #2** — the key combines `4x + 4x − 10x` into `−10x`; that sum is `−2x`,
  which changes the answer from `−17/10` to `−17/2`.
- **0B HW1 #2** — the key adds `5041 + 1225` and writes `√6226`; the sum is `6266`.
- **Re-take #2** — the key gets `P(0, 28)` right but gives `3x − y = −28`, which
  has slope 3 and is not perpendicular to AB (slope `−3/4`). The perpendicular
  is `4x − 3y = −84`, with x-intercept `−21`, not `−28/3`.
- **Factoring 03 #8** — the key factors `(x² − 4)²` as `[(x+4)(x−4)]²`; `x² − 4`
  is `(x+2)(x−2)`.
- **Real Deal 04 #5** — the key writes the shared binomial as `x − 2` instead of
  `x² − 2`, so its answer `(x−2)(x−3)(x²+3x+9)` is degree 4, not 5. The correct
  factoring is `(x²−2)(x−3)(x²+3x+9)`.
- **Factoring Techniques 05 #8** — the key's working line is right,
  `(x⁸+9)(x⁴+3)(x⁴−3)`, but the boxed answer `(x⁸+9)(x⁴+9)(x²+3)(x²−3)`
  multiplies out to `x¹⁶ − 72x⁸ − 729`.

The Lines solutions follow the teacher's own steps from the keys: a right
triangle and a proportion for segment ratios, one slope set equal to the
negative reciprocal of the other for perpendiculars, and expand-then-factor (or
the quadratic formula) when a letter is being solved for.

For Factoring, every answer was also checked to be fully factored. Problem
labels are by sheet: `F02`, `F03`, `RD01`, `RD02`, `RD04`, `FT05`. Part I of
*Factoring 02* asks for the factored form, but its key only fills in the missing
term, so those factored forms were added here.

No key was supplied for *The Basics of Unit 0B*, so those six answers are
verified but not compared. In **#1** both `k = 4` and `k = 2` work; `k = 2`
makes one line vertical and the other horizontal, so it has to be checked in
the original equations rather than with slopes.

One more is a judgment call rather than an error: **0A 05 #5** boxes both roots
of the continued fraction, where the quiz-review key for the same pattern rejects
the negative one. The guide rejects it and explains why.

## Structure

`index.html` is self-contained — no build step, no dependencies to install.
Styles and scripts are inline; the graphs are hand-generated inline SVG that
follows the light/dark theme. MathJax is the one external resource, loaded from
a CDN at view time.
