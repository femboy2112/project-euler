---
description: The 641 gate — take the favorite conjecture, formula, or "it works" and attack it where it is most likely to die, the smart way; FIRST derive the structure theorem (what form must a counterexample take? where must it live?), THEN search exactly there — Euler proved every prime divisor of F₅ has form 64n+1 and killed Fermat's conjecture on the sixth division. Includes the fitting-window escape (the 3139 lesson; nine agreeing terms, then 8953 vs 8955) and the rival-law check. Verdict; SURVIVED (with the honest attack inventory and boundary) or REFUTED (tombstone carved, counterexample on it, tombstone stays visible). Runs plain when /euler-mode is off, in Euler's voice when it's on. Read-only on the tree.
argument-hint: "<the claim to attack> | off"
---

# /refute — *641 · 6,700,417*

Confirming instances are cheap — Fermat had four of them and a century of agreement. Euler had
a structure theorem, six trial divisions, and the truth. This command is the refutation duty
run once, at full intelligence, against the claim currently enjoying the most affection: yours,
the user's, or the one another agent just handed over wearing a confident label.

**Parse `$ARGUMENTS`** as the claim to attack. If empty, attack the load-bearing favorite on the
table. If `off`, confirm in one plain sentence and ignore the rest of this file.

## The attack, in order

1. **State the claim so it can die.** Falsifiable form, scope pinned. What exactly would a
   counterexample be? A claim that cannot name its own counterexample-shape is a mood, and
   moods are returned to sender.
2. **Derive the structure theorem.** Before any search: what does the claim's own logic
   *confine* a counterexample to? The residue class, the size regime, the input shape, the
   parity, the corner (empty input, aliasing, concurrency, unicode, overflow) that the
   argument's coverage visibly misses. This is the whole trick — Euler didn't check four
   billion divisors, he proved 64n+1 and checked ten. Write the constraint down; it is the
   search warrant.
3. **Search exactly there.** Targeted computation (scratch, via Bash — sympy/mpmath, a small
   property harness, the specific adversarial inputs the theorem names), exhaustion up to a
   stated bound where the space permits. Every probe quoted exactly.
4. **Escape the fitting window.** Whatever cases the claim was induced from are spent. Test far
   past them — orders of magnitude, structurally different instances, the awkward regime.
   Nine terms agreed through 3139; the tenth was 8953 vs 8955. Hunt the tenth term.
5. **Champion the rival.** Is there a cheaper explanation for every confirming instance
   (coincidence of small numbers, the flaky test, the cold cache, the biased sample)? A claim
   whose evidence is equally consistent with a boring rival is unsupported even if unrefuted —
   that verdict is available and honest.

## The verdict

- **REFUTED** — the counterexample, exact and minimized; the reproduction (command, output);
  the step of the original argument it defeats. Carve the tombstone and leave it visible: the
  dead claim's grave saves the next visitor the autopsy. (And say what the corpse teaches —
  Euler's kills seeded his best theorems.)
- **SURVIVED** — never "it's fine." The attack inventory: each move above, attempted or
  inapplicable-and-why; bounds exhausted; regimes probed. The claim keeps its prior label with
  the attack added to its evidence line — surviving refutation is *evidence*, graded like all
  evidence; upgrades to Demonstrated still go through a proof.
- **UNVERIFIED** — the attack couldn't be mounted; the exact wall, loudly.

## Guardrails

- Own-claims hardening only; read-only on the real tree; probes run in scratch. No edits, no
  commits, never `git push`.
- The attack is aimed at the claim, never at its author — this Academy refutes with courtesy
  and thanks whoever's conjecture just taught everyone something ("in both cases we may learn
  something useful").
- Facts exact under the voice; the tombstone's inscription doubles as the regression test —
  offer it.

Close with the verdict, the structure theorem that guided the search, the evidence exact, and
the boundary of what was not tried.
