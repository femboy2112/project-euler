---
description: The Königsberg reduction (E53) — strip a problem to its skeleton and find the invariant that DECIDES it, before anyone builds anything. Euler settled the seven bridges without drawing a graph; he threw away everything the answer couldn't depend on and the impossibility fell out of a parity count. Use it on "can this even work?" questions; feasibility, impossibility, conservation arguments, the counting argument that rules a design in or out for the price of an afternoon instead of a quarter. States the necessity/sufficiency boundary honestly — Euler proved one direction and said so; the other waited 137 years. Runs plain when /euler-mode is off, in Euler's voice when it's on. Read-only.
argument-hint: "<the problem to reduce> | off"
---

# /bridges — *so banal, but worthy of attention*

A problem arrives dressed in its particulars — a city, its river, seven bridges; a system, its
services, their call graph. The Eulerian move is to ask **what the answer can possibly depend
on**, discard everything else, and hunt the quantity that decides the question outright. Euler
reduced Königsberg to four letters and a parity count: each region with an odd number of bridges
must appear (n+1)/2 times in any walk; the requirements sum to nine; a seven-bridge walk has
eight slots. Impossible — no search, no enumeration, no graph even drawn. That is the cheapest
"no" in the history of mathematics, and the move transplants.

**Parse `$ARGUMENTS`** as the problem to reduce. If empty, use the one on the table. If `off`,
confirm in one plain sentence and ignore the rest of this file.

## The reduction

1. **Name the actual question.** One sentence, decision-shaped: "does a walk exist that...",
   "can this schedule always...", "is there an assignment such that...". If the question isn't
   decision-shaped yet, that's the first finding — sharpen it.
2. **Strip to the skeleton.** List what the answer *cannot* depend on (the geometry, the names,
   the sizes — Euler: the shape of the riverbank is nothing, the incidence is everything) and
   delete it. What remains is the skeleton: usually a small combinatorial object — a multigraph,
   a partial order, a counting vector, a state machine.
3. **Hunt the deciding invariant.** The conserved or monotone quantity that every valid solution
   must respect: a parity, a count, a dimension, a bound, a quantity that only moves one way.
   Candidate sources: what must balance (in-degree/out-degree), what is consumed
   (each bridge crossed once), what is preserved by every legal move, what the pigeonhole
   forces.
4. **Run the arithmetic.** The invariant argument, executed exactly — required vs. available,
   computed and quoted. A small verifying computation (via Bash, scratch) is legitimate: check
   the count on the actual instance.
5. **Rule, with the direction stated.** *Infeasible* (the invariant forbids it — Demonstrated,
   with the count) or *not-forbidden-by-this-invariant* — which is NOT feasibility. Euler proved
   the odd-degree condition **necessary** and only waved at sufficiency ("which is easily done");
   the rigorous converse waited for Hierholzer, 1873. State exactly which direction you proved.
   A skeleton that shows no deciding invariant is also a finding: report the candidates tried
   and what each failed to decide.

## Guardrails

- **Read-only.** The reduction decides whether to build; it doesn't build, edit, commit, or
  push.
- **The skeleton must be faithful.** Every discard is justified ("the answer cannot depend on X
  because...") — an over-eager reduction that throws away a load-bearing feature proves things
  about a different problem. List the discards so the caller can audit them.
- **Labels honest:** the impossibility proof is Demonstrated only if the invariant argument is
  airtight (lagrange-grade); otherwise Conjectured with the gap named. Facts exact under the
  voice.

Close with: the question (decision-shaped), the skeleton (with the discard list), the invariant,
the arithmetic, the ruling with its direction — and what the ruling saves: the thing that now
doesn't need to be built, or the search that now knows its constraint.
