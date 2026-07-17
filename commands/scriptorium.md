---
description: The scriptorium — blast a broad front of trivial, independent, homogeneous chores with a swarm of Fuss-scribes, one per unit; a lint fix across 200 files, a docstring per function, a table regenerated per dataset, a check run per module. Each scribe gets ONE bounded unit with a pass/fail check, never self-certifies past the trivial, and hands oversized units back up; the whole front is verified as a whole before it is called cleared. Refuses non-fronts; units with cross-dependencies or judgment get WORSE under a swarm — those go to the proper Academy member instead, and this command says so rather than convene. Runs plain when /euler-mode is off, in Euler's voice when it's on.
argument-hint: "<the front: many homogeneous units> | off"
---

# /scriptorium — *Mr. Golovine worked on more than 70 mémoires, and there were over 250 others*

The blind Euler ran a scriptorium: sons, students, and one very patient tailor's apprentice,
each handed bounded pieces of calculation while the design stayed at the master's desk. That is
the only shape of work a swarm improves: **many units, each trivial, each independent, each
checkable**. This command runs that scriptorium once, against one front.

**Parse `$ARGUMENTS`** as the front. If `off`, confirm in one plain sentence and ignore the rest
of this file.

## First — is it actually a front?

A front is: units that are **homogeneous** (same operation each time), **independent** (no unit
changes another's input), **trivial** (no judgment inside a unit), and **checkable** (a
pass/fail per unit). Test the front before convening:

- Cross-dependencies → not a front; it's a sequence. Route to `daniel` or handle in order.
- Judgment inside units (two scribes would do it differently) → not a front. Route to the
  proper member (`the-princess` for prose, `lagrange` for anything touching proof logic).
- Fewer than ~10 units → not worth a scriptorium; do it directly.

**Refusing is a valid outcome** — say why, name the right shape, stop. A swarm applied to a
non-front produces 200 individually-plausible wrongs.

## The scriptorium

1. **Enumerate the units.** Explicitly (glob, grep, list) — the roster is the contract, and the
   count is stated up front. Silent truncation is banned; if you cap, say what was dropped.
2. **Define the unit spec once.** The exact operation, the exact pass/fail check, the exact
   hand-back rule ("if the file contains X, stop and return it"). Every scribe gets the same
   spec — that's what homogeneous means.
3. **Dispatch the swarm.** One `project-euler:fuss` per unit (parallel, label
   `'Fuss - <unit>'`), each briefed with its single unit + the spec + the Iron Rule. Scribes
   never self-certify past the trivial: each returns its diff summary, its check's exact
   output, or its hand-back note.
4. **Collect the hand-backs.** Units that came back up are the interesting residue — triage
   them yourself (they were bigger than they looked, which is information about the front).
5. **Verify the front as a whole.** Per-unit checks passing is necessary, not sufficient: run
   the whole-front check (the full lint pass, the build, the suite, the row-count
   reconciliation) yourself, and quote it. A front is cleared when the *whole* is Observed
   clean, not when the parts self-reported.

## Guardrails

- Write scope: exactly the enumerated units, scratch aside. **No commits, never `git push`** —
  the cleared front is staged for the Correspondent's imprimatur.
- Scribe reports are testimony: spot-check a sample at your own desk (a few units, re-read
  directly) before certifying the front; state the sample size.
- Facts exact under the voice: unit counts, pass/fail tallies, and the whole-front check output
  are quoted, not summarized into optimism.

Close with: the roster count, per-unit tally (done / handed-back / failed), the hand-back
triage, the whole-front verification quoted, and the staging note for the imprimatur.
