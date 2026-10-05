# Algebra pattern guide

A single-page study guide built from worked problem sheets. For each sheet it
records the *pattern* behind the problems — the visual cue that tells you which
method applies — alongside every problem solved step by step.

**Live site:** https://wm.github.io/algebra-two/

## Contents

The page has two topics, switched at the top:

- **Equations** — clearing denominators, distributing awkward coefficients,
  rational equations, substitution, infinite continued fractions, quadratics.
  Built from *Unit 0A 05* and *0A 06 Quiz Review 2*.
- **Lines** — slope, the three forms of a line, perpendiculars, midpoint,
  partitioning a segment by a ratio, distance, and distance from a point to a
  line, intercepts, intersections, and solving for an unknown coordinate or
  coefficient. Built from *0B Homework 1*, *Distance from a point to a line*,
  *Graphing Lines Review 2*, *The Basics of Unit 0B*, and the
  *Unit 0B 10-Problem Review*.

Each topic has three tabs: a decision **Checklist**, the **Patterns** with their
cues, and the **Solved problems** with collapsible solutions.

The Lines topic has a fourth tab, **Practice test**: ten new problems modelled
on the 10-Problem Review, with different numbers and in a different order, each
with a hidden worked solution. These were written for the guide and are not
from the teacher.

## Notes on the answers

Every solution was worked by hand and then verified symbolically with SymPy.
Two answers disagree with the teacher's keys, and both are flagged inline on the
problem itself:

- **0A 05 #2** — the key combines `4x + 4x − 10x` into `−10x`; that sum is `−2x`,
  which changes the answer from `−17/10` to `−17/2`.
- **0B HW1 #2** — the key adds `5041 + 1225` and writes `√6226`; the sum is `6266`.

The Lines solutions follow the teacher's own steps from the keys: a right
triangle and a proportion for segment ratios, one slope set equal to the
negative reciprocal of the other for perpendiculars, and expand-then-factor (or
the quadratic formula) when a letter is being solved for.

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
