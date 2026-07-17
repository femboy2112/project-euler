---
description: Euler's re-proving habit as a one-shot gate — run a load-bearing claim through N independent BLIND derivations (default 3) and accept only the consensus, with disagreement surfaced as signal rather than averaged away. Euler gave three proofs of Basel in E41 alone and kept producing routes for twenty years, because a result reachable only one way is fragile. Each bearing works by its OWN method, blind to the original reasoning and to its siblings. Runs plain when /euler-mode is off, in Euler's voice when it's on. Read-only on the tree; verdict only.
argument-hint: "<the claim to re-derive> [N] | off"
---

# /second-proof — *he never rested in his search for better proofs*

A claim is about to bear weight — a value about to be certified, a fix about to ship, a
conclusion about to become a premise. It was derived once. Euler's rule: a result that has been
reached only one way has been reached *almost* zero ways; he re-proved his own theorems for
decades ("more natural," "simpler," "more direct") and each new route either strengthened the
result or exposed the crack the first route had stepped over.

**Parse `$ARGUMENTS`** as the claim (and optional bearing count N, default 3). If empty, use the
load-bearing claim on the table. If `off`, confirm in one plain sentence and ignore the rest.

## The gate

1. **State the claim falsifiably.** One sentence with scope — what would have to be false for
   it to be wrong. If it can't be stated so it can fail, that finding ends the gate early.
2. **Design N blind bearings, methods first.** Each bearing gets a *different* route: a
   different algorithm, a different tool/library, a different formulation (symbolic vs numeric,
   direct vs contrapositive, analytic vs combinatorial), a different entry point into the code.
   Independence is structural: **no bearing sees the original derivation or another bearing's
   work** — a route that reads the first route's steps inherits its bug and counts as an echo.
3. **Spawn the bearings in parallel.** `project-euler:daniel` for computational routes (each
   with its own Instrument calibration), `project-euler:lagrange` for proof-shaped routes —
   labels `'Daniel - bearing 2: mpmath route'` etc. Each is briefed with the claim and its OWN
   method only, and returns: verdict, method, evidence with exact values, confidence, boundary.
4. **Tabulate — consensus and splits.** Where all bearings agree, the claim earns its upgrade:
   **Demonstrated** (engineering register: independent witnesses) or a heavily-armored
   Conjectured, per what the routes can actually establish. Where they split: **the split is
   the finding.** Do not average. First run the dumb-cause reconciliation (precision mismatch,
   different edition of the input, an off-by-one in scope) — then, if the split survives, it is
   real signal: at least one route has a hole, and finding it usually teaches more than the
   original claim was worth.
5. **Rule.** Confirmed-by-consensus (with the N routes named), or SPLIT (with the disagreement
   map and the next discriminating check), or UNVERIFIED (bearings couldn't run; the exact
   walls). Boundaries stated: what the consensus does *not* cover.

## Guardrails

- **Blindness is structural, not polite.** The spawn prompts contain the claim, never the
  reasoning that produced it. If true blindness is impossible (the claim IS the reasoning),
  say so — the gate degrades honestly to an audit and is labeled as one.
- **N scales with stakes.** A hangnail doesn't convene three bearings; a number about to be
  published might deserve five. Say what you chose and why.
- Read-only on the real tree; bearings compute in scratch. Facts exact under the voice; never
  `git push`.

Close with: the claim, the bearings (method + verdict + evidence each), the consensus or the
disagreement map, the label the claim now honestly wears, and its boundary. Two witnesses
establish; one witness with an echo does not.
