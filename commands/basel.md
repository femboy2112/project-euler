---
description: The flagship single-problem arc, run on E41's verified anatomy — take ONE hard question (a closed form to find, a mystery constant, a root cause with mathematical bones) and hunt it the way Euler took the Basel problem; numerics FIRST to many digits (get the answer before its form), then the audacious analogy or structural hunt for what the number IS, then PAY for the guess (recover known results by the same method, verify fresh predictions, cross-check by an independent route), then the demonstration attempt, then publish the path. Runs plain when /euler-mode is off, in Euler's voice when it's on.
argument-hint: "<the hard question> | off"
---

# /basel — *now, however, quite unexpectedly, I have found an elegant formula*

The Basel problem stood for ninety years because everyone hunted the *form* before knowing the
*value*. Euler inverted it: he built convergence acceleration, computed ζ(2) = 1.644934... to
many digits, and only then could recognize π²/6 when a daring method produced it — and only
then did he trust the method, because it also re-derived Leibniz's known series and predicted
ζ(4) = π⁴/90, which checked. This command is that arc, run once, end to end.

**Parse `$ARGUMENTS`** as the hard question. If empty, use the one on the table. If `off`,
confirm in one plain sentence and ignore the rest of this file.

## The arc

1. **Stage 0.** Known result? Known constant? (An unrecognized number goes to an inverse
   symbolic check — is it π²/6, log 2, γ, a simple combination? — before any original hunt.)
2. **Numerics first.** Get the answer to many digits before hunting its form — build/calibrate
   the instrument, accelerate the computation if it crawls (Euler built Euler–Maclaurin *because*
   direct summation needed a million terms). For a non-numerical mystery: pin the phenomenon
   precisely (exact failing input, exact measurements) before theorizing. Spawn
   `project-euler:daniel` when the computation is real work.
3. **The daring guess.** Hunt what the answer IS: pattern-match the digits, make the audacious
   analogy (treat the infinite like the finite, the discrete like the continuous — *labeled*),
   find the structural reframe. State the conjecture falsifiably, with its fitting window marked.
4. **PAY for it — the E41 payment schedule, all three installments:**
   - **(a) Match the digits.** The conjectured form agrees with the precomputed value to full
     precision.
   - **(b) Recover a known truth.** The same method/analogy re-derives something already
     established ("if our method should appear to some as not reliable enough, a great
     confirmation comes to light here").
   - **(c) Verify a fresh prediction.** The method predicts something new and checkable — check
     it, preferably by an independent route.
   Any installment that fails is reported as loudly as success; an unpaid analogy stays a
   speculation, not a finding.
5. **The demonstration attempt.** Spawn `project-euler:lagrange` (or attempt directly): proof,
   or the honorable report of exactly which lemma is missing. Optionally send the survivor
   through `project-euler:dalembert` first — a conjecture that survives directed refutation is
   worth a proof attempt; one that doesn't just saved you the effort.
6. **Publish the path.** The memoir: value, conjecture, payments, proof or gap, false starts
   included — labeled throughout.

## Guardrails

- Twenty digits moved Euler to *conjecture*, not to claim. **Numerical agreement never upgrades
  to Demonstrated** — the arc's whole point is that the payment buys confidence and the proof
  buys certainty, and the Ledger tells them apart.
- Sandbox any formal manipulation; label it formal at every appearance.
- Facts exact under the voice; never `git push` without explicit say-so.

Close with the memoir: the question, the value (digits stated), the conjecture and its label,
the three payments with results, the demonstration or the named gap, and what remains open.
