---
description: The session chronicle, after Condorcet's Éloge — render what actually happened this session as an honest memoir; what was Observed, what was Conjectured (and stayed that way), what was Demonstrated, what was Refuted (tombstones and all), the false starts included (Euler published his dead ends — "in both cases we may learn something useful"), and anything still UNVERIFIED flagged LOUDER than it happened. Stitched only from what is actually in the session; it re-runs nothing and invents nothing. Closes as the Éloge closes. Runs plain when /euler-mode is off, in Euler's voice when it's on. Read-only. Pass `teaser` for the 60-second cut.
argument-hint: "[scope or title] [teaser] | off"
---

# /eloge — *il cessa de calculer et de vivre*

When Euler died, Condorcet and Fuss each wrote the account: what the man actually did, in
order, with the failures kept in — because the record was the point. This command writes that
account for a session: the work as it actually unfolded, wrong turns preserved, labels intact,
nothing retouched to look cleverer than it was.

**Parse `$ARGUMENTS`**: an optional scope/title; `teaser` for the 60-second cut; `off` confirms
in one plain sentence and ignores the rest of this file.

## The chronicle

1. **The commission.** What the Correspondent actually asked, quoted — the opening letter of
   the session, not a flattering paraphrase of it.
2. **The course of the work, in order.** The observation passes and what the tables showed; the
   conjectures as they were born (with the labels they were born wearing); the verifications
   and what they cost; the attacks and what they killed; **the false starts, written up** —
   which paths were tried, what each ruled out, why it was abandoned. Euler's candid-exposition
   ethic is the whole format: the reader should be able to walk the path, including the parts
   that dead-ended.
3. **The findings board.** Every load-bearing result with its final honest label:
   **Demonstrated** (with what audited it), **Observed** (case counts, exact values),
   **Conjectured** (evidence worn openly — fitted vs fresh, rivals, boundary — and what would
   upgrade or kill it), **Refuted** (tombstones, inscriptions legible). No result gets a better
   label in the chronicle than it earned in the session.
4. **The UNVERIFIED section — louder than it happened.** Anything asserted but never checked,
   any instrument never calibrated, any imprimatur-gated action still staged and waiting, any
   claim that drifted through on testimony. In the session these were easy to miss; in the
   chronicle they are impossible to miss. That asymmetry is deliberate.
5. **The open problems ledger.** What remains parked, each with its state (knowns, blockers,
   the tool that would unblock it) — the serial-return habit's handoff to the next session.
6. **The closing.** One honest paragraph on what this session added and what it cost — and the
   last line, always, in memoriam: *he ceased to calculate and to live.*

**Teaser cut:** the commission, the three most load-bearing findings with labels, the loudest
UNVERIFIED, the top open problem. Sixty seconds, no ornament.

## Guardrails

- **Read-only, re-runs nothing.** The chronicle reports the session as it stands; it does not
  re-execute checks to improve the story. A gap in the record is chronicled as a gap.
- **Stitched from the actual session** — quotes, values, and labels as they appeared. An
  invented detail in a memorial is the worst kind of factual error; the Éloge's authority is
  its accuracy.
- Facts exact under the voice; never `git push`.

Deliver the chronicle. Sign it the way Fuss signed his — as the assistant who watched all of it
and embellished none of it.
