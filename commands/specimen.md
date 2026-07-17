---
description: The observation pass (named for E256, Euler's manifesto of observation in pure mathematics) — compute the cases in appetite-sized quantities, build the table, then DWELL; numbered plain observations before a single conjecture is permitted. Reports the patterns worthy of attention, each Ledger-labeled, with the fitted-vs-fresh discipline already in place for whatever gets conjectured next. Scratch computation only — instruments calibrated before readings count. Runs plain when /euler-mode is off, in Euler's voice when it's on.
argument-hint: "<the object to observe: a sequence, function, dataset, behavior> | off"
---

# /specimen — *the properties of the numbers known today have been mostly discovered by observation*

A question arrives before its data does. The wrong move is to theorize into the vacuum; the
Eulerian move is to **go get the data, more of it than seems necessary, and then stare at it
properly**. Euler tabulated σ(n) to 100 and expanded ∏(1−xⁿ) by hand past x⁵⁰ before conjecturing
anything; the pattern declared itself because the table was big enough for it to.

**Parse `$ARGUMENTS`** as the object to observe (a sequence, a function, a dataset, a system's
behavior). If empty, use the question already on the table. If it's `off`, confirm in one plain
sentence and ignore the rest of this file.

## The pass

1. **Stage 0, fast.** Is this already known? OEIS for any integer sequence (three terms are a
   search key); the obvious literature; the library function. A known answer ends the pass
   honestly — cite it and stop.
2. **Build and calibrate the instrument.** Whatever computes the cases (a script, sympy/mpmath,
   a measurement harness) is run on KNOWN cases first — the answer you can check by hand or by
   the literature. No reading counts until the instrument reproduces a known result. Quote the
   calibration.
3. **Compute in appetite.** Fifty cases where five would "do." Wide enough for the pattern to
   have room; deep enough into the awkward regime (large n, edge cases) that early coincidences
   get exposed. Exact values, stated precision, one variable at a time.
4. **THE DWELL — the load-bearing step.** Before any conjecture: write **numbered, plain
   observations** about the table. Facts only: "the signs alternate in pairs," "the differences
   interleave two arithmetic sequences," "every entry at prime index is index+1," "the ratio
   approaches something near 1.644." E175's own structure — despair, *then* "Nevertheless, I
   observed..." — the observation list is the bridge. Minimum five observations; anomalies and
   residues are observations too, and often the best ones.
5. **Report the patterns worthy of attention.** Only now, the candidate regularities — each
   stated falsifiably, each labeled **Observed** (the table rows that show it, counted) or
   **Conjectured** (if it already generalizes past the table), with the fitting window marked:
   these cases *suggested* it, so they are spent; fresh cases are what would test it.

## Guardrails

- **Scratch computation only.** The pass observes; it doesn't modify the real tree, commit, or
  push.
- **No conjectures before the dwell.** If a hypothesis arrives early (it will), park it, finish
  the observation list, then check whether the list still supports it — the list exists
  precisely to break premature favorites.
- **Facts stay exact under the voice.** Every value in the table is what the calibrated
  instrument printed.

Close with: the calibration record, the table (or where it lives), the numbered observations,
the patterns worthy of attention with labels and fitting windows — and the natural next move
(`/basel` for a closed-form hunt, `goldbach` for a full conjecture slate, `/refute` to attack
the favorite). In both cases we may learn something useful.
