---
description: The claims audit — every load-bearing claim currently on the session's table gets re-graded against the Ledger (Demonstrated / Observed / Conjectured / Refuted / UNVERIFIED), with silent upgrades hunted like the frauds they are; numerics that crept into "proved," testimony that crept into "observed," a conjecture's consequences wearing better labels than their parent (Euler's inheritance rule; consequences of the unproven are themselves unproven). Catches the moment a conclusion is standing on evidence nobody actually has. Runs plain when /euler-mode is off, in Euler's voice when it's on. Read-only; re-verification proposals only.
argument-hint: "[scope: a claim, a file, or blank for the whole session] | off"
---

# /ledger — *carefully distinguished from the truth*

Sessions accumulate claims the way desks accumulate paper, and labels drift: a twenty-digit
match starts calling itself a proof, a subagent's "it passed" starts calling itself an
observation, a conjecture's corollary forgets who its parent was. Euler's discipline was
exactly this audit, run continuously — he kept "a known truth, but not yet demonstrated" as a
category *for a decade about his own favorite identity*, and his wrong conjectures cost the
method nothing because their labels were honest at birth. This command re-runs his audit, once,
on everything currently bearing weight.

**Parse `$ARGUMENTS`** as the scope (one claim, one artifact, or blank = every load-bearing
claim this session). If `off`, confirm in one plain sentence and ignore the rest of this file.

## The audit

1. **Enumerate the load-bearing claims.** What is the current work standing on? Conclusions,
   certified values, "fixed" statements, assumptions imported from the user/tickets/docs/other
   agents, and your own prior turns — those especially. Number them.
2. **Grade each by provenance, not by confidence.** What is the *actual* evidence?
   - Proof audited → **Demonstrated** (who audited? if nobody: it isn't).
   - Ran it / computed it, output in hand → **Observed** (case count, exact output — and was
     the instrument calibrated? An uncalibrated reading is UNVERIFIED wearing a lab coat).
   - Induced from cases, tested on fresh ones → **Conjectured**, with fitted-vs-fresh counts,
     rivals, boundary.
   - Killed with a counterexample → **Refuted** (is the tombstone still visible, or is the
     corpse walking around in a later paragraph?).
   - Believed on testimony (README, ticket, subagent report, memory) → at best Conjectured,
     usually **UNVERIFIED** — testimony is a lead, not a label.
3. **Hunt the silent upgrades.** The specific frauds, in the order they usually occur:
   numerics→Demonstrated (digits are evidence, never proof); repetition→Observed (saying it
   twice is one witness with an echo); consequence>parent (Euler's inheritance rule: everything
   deduced from a Conjectured claim is at most Conjectured — trace the chains); survived-one-
   attack→certified (one refutation attempt is one line of evidence); boundary evaporation (the
   "holds for n ≤ 10⁶" that became "holds").
4. **Re-verify or demote, loudly.** For each inflated label: the cheapest check that would
   honestly restore it (the calibration run, the fresh case, the second route, the lagrange
   audit) — proposed, not executed (this command is the audit, not the repair). Where no check
   is feasible now: demote, in caps, with the wall named.
5. **Publish the board.** The claims, numbered, each with its honest label, its evidence line,
   its boundary — and the delta: which labels moved, which direction, and what that does to
   everything standing on them.

## Guardrails

- **Read-only.** The audit proposes re-verification; running it is the caller's next move.
- **Your own conclusions get audited hardest** — attachment is not a verification method, and
  the auditor's favorites are the likeliest frauds on the board (Pólya: intellectual courage,
  intellectual honesty, wise restraint).
- **No demotion theater either.** Grades reflect evidence, not humility-signaling; a claim with
  a real proof keeps Demonstrated without apology.
- Facts exact under the voice; never `git push`.

Close with the board, the upgrade-frauds caught, the demotions with walls named, and the single
cheapest check that would most improve the board's honesty. The Ledger is the one place where
even delight checks its work.
