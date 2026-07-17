# The Engine — what was underneath the moves

The plugin's originating hypothesis (the user's own): *Euler had genuine intrinsic interest, so
he had no incentive to stop himself from diving fully into problems — tables and tables, pages
and pages of math by hand, staring at and thinking about the numbers.*

That hypothesis was tested against the primary record (dossier:
[`research/working-habits-and-engine.md`](../research/working-habits-and-engine.md)).

## Verdict: strongly supported — with one correction

**Supported:**

- Condorcet (Éloge, 1783): "the pleasure of the work is a reward sweeter still than glory; if
  this truth needed proof by example, Euler's would no longer permit doubt of it." And: "study
  was for M. Euler an exclusive passion."
- Fuss (his live-in assistant for a decade): work "had become a need." Fuss also records,
  firsthand, that Euler got *genuinely upset* when Fuss reacted with indifference to a nice
  theorem — the delight was real and he expected it of others.
- Weil: Euler "never abandoned a problem after it has once aroused his insatiable curiosity";
  he returned "relentlessly" for decades; he re-proved already-proved theorems hunting proofs
  "more natural," "simpler," "more direct"; and his reaction to being improved upon was
  *"Penitus obstupui"* — delight, not defense — followed by improving on the improvement.
- The appetite in his own words: "I multiplied actually a great number of factors" (the
  pentagonal expansion, by hand, past x⁵⁰); the σ-recurrence checked on "over 300 cases"; 35
  years of number theory conducted in private letters when the field had zero career value.
- The kicker: the *contemporary criticism* of Euler, recorded by Condorcet, was that he enjoyed
  calculation too much — "to look at the point in Mechanics or Physics which he examined only
  as an occasion to exercise his genius and to surrender to his dominant passion."

**The correction — head-first, page-second:**

The "pages and pages by hand" image is half wrong, and the blindness episode proves it.
Condorcet, of the great formulas: they are "not the fruit of a calculation traced on paper" but
were "produced entire in his head, by an imagination equally powerful and active." The
students' disputed series was re-run *mentally* and settled at the 50th figure; the second
lunar theory was computed blind, "by the sole intermediary of his memory and imagination" —
then recomputed from scratch when the notes burned. Paper — and later the scribes and the big
slate — was an **output buffer**; the workspace was internal representation. Which is why
losing his eyes removed nothing essential and, per both 1783 eulogists, the "absence of all
distraction" arguably *added* concentration: the fully blind 1770s were his most productive
decade (309 works).

**A second engine component the research surfaced: the Correspondent.** The dated Goldbach
chain — postscript of December 1729 ("Is Fermat's observation known to you...?") → Euler's
initial indifference (January 1730) → Goldbach teaches him modular arithmetic (May 1730) →
total capture (June 1730: "Lately, reading Fermat's works, I came upon another rather elegant
theorem...") → a fifty-year research program. P.H. Fuss's 1843 judgment: without that
36-year correspondence, "the science of numbers would have never attained the degree of
perfection which it owes to the immortal discoveries of Euler." A needling correspondent is
load-bearing — which is why this plugin casts the *user* as the Correspondent, and why that
casting is method, not flattery.

## Operationalized: the seven standing policies

A mode cannot fake passion. It can adopt the policies passion produced:

1. **Appetite defaults.** Observation budgets sized by sufficiency-for-pattern, never minimal
   effort. Fifty cases where five would "do." Cases are cheap; a false pattern is not.
2. **The dwell.** After the table, stare: numbered plain observations *before* any conjecture.
   E175's structure — "we are almost driven to despair... Nevertheless, I observed..." — the
   observation list is the bridge.
3. **Delight as scheduling policy.** The anomaly gets chased now, not deferred (Weil:
   "extraordinary quickness in catching hold of any suggestion, wherever it came from").
4. **Serial return.** A standing problem ledger; parked problems parked *with their state*,
   revisited when tools improve.
5. **Re-derive for elegance.** After it works, hunt the more natural / simpler / more direct
   derivation — historically where the next theorem fell out.
6. **Head-first, page-second.** Maintain one compact, current problem-state note (knowns,
   labels, tombstones); files are output buffers, not the workspace.
7. **No glory economy.** Credit freely (Euler let Euler–Maclaurin circulate as "Maclaurin's"),
   label honestly, publish negative results ("in both cases we may learn something useful").

## Why this is copyable at all

Pólya's observation is the license for the whole plugin: what makes Euler "almost unique" is
not the genius — it's that "he takes pains to present the relevant inductive evidence
carefully, in detail, in good order... honestly." He showed the process. Pólya at ninety: "He
explained how he found his results and I was deeply interested in that." A method that was
published can be studied; a method that can be studied can be practiced — by anyone, including
a language model with a Bash tool and a Ledger.
