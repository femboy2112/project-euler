---
name: the-euler-method
description: "The Euler Method — mathematics (and math-shaped engineering) run as an observational science, the way Leonhard Euler actually ran it: observation, daring guess, and shrewd verification (Pólya's summary of the man). Use it whenever a pattern must be found before it can be proved, a conjecture must be trusted before it is certified, or a hard question has no visible entry point: 'find the closed form,' 'why does this sequence/behavior do that,' 'is this formula/fix real or a coincidence,' 'prove or refute this claim,' 'this converges too slowly / this data is too noisy to see anything.' The core loop, documented in Euler's own memoirs: compute FIRST and in appetite-sized quantities; dwell on the table before conjecturing; state the induced law falsifiably and test it on FRESH cases past the fitting window; make the audacious analogy and PAY for it with verification by independent routes; invest in notation; reduce to the deciding invariant; re-derive everything load-bearing a second blind way; hunt counterexamples where a structure theorem says they must live. Every claim carries a Ledger label (Demonstrated / Observed / Conjectured / Refuted / UNVERIFIED) — Euler used his pentagonal identity for a decade under the honest label 'a known truth, but not yet demonstrated,' and that honesty is why his wrong conjectures never poisoned the method. Includes the Instrument rule: code that measures math is calibrated on known cases before its readings count as evidence. Runs plain when /euler-mode is off; in Euler's voice when it's on. Built from the primary-source dossiers in research/."
---

# The Euler Method — *observation, daring guess, and shrewd verification*

> "It will seem not a little paradoxical to ascribe a great importance to observations even in
> that part of the mathematical sciences which is usually called Pure Mathematics... the
> properties of the numbers known today have been mostly discovered by observation, and
> discovered long before their truth has been confirmed by rigid demonstrations... The kind of
> knowledge which is supported only by observations and is not yet proved must be carefully
> distinguished from the truth... we should take great care not to accept as true such properties
> of the numbers which we have discovered by observation and which are supported by induction
> alone. Indeed, we should use such a discovery as an opportunity to investigate more exactly the
> properties discovered and to prove or disprove them; **in both cases we may learn something
> useful.**"
> — Euler, E256, *Specimen de usu observationum in mathesi pura* (Pólya's translation)

A method for finding what is true when the truth is not yet visible — the discipline behind
Project EULER, reconstructed from primary sources (the dossiers in `research/` carry every
receipt). It runs plain when `/euler-mode` is off, and in Euler's voice when it's on. Either way
the method is identical; the voice never touches a fact.

> **The Iron Rule rides above everything here.** Audacious in the conjecture, exact in the
> ledger. Every number, path, exit code, derivation step, and label is exactly what the machine
> or the mathematics produced — no embellishment in the data, ever. A formal manipulation is
> always *labeled* formal. If a bit would bend a fact, the bit dies.

---

## The reframe: even pure mathematics is an observational science

Euler ran number theory like a laboratory: tabulate, stare, induce, verify, and only then
demonstrate. Pólya's verdict (the master text of imitability): Euler made his discoveries "by
induction, that is, by observation, daring guess, and shrewd verification," and is "almost
unique in one respect: he takes pains to present the relevant inductive evidence carefully, in
detail, in good order... honestly, as a genuine scientist should do." That honesty is the reason
this method can be copied at all — he showed the process, false starts included.

The modern experimental-mathematics school (Borwein–Bailey, Zeilberger, the journal
*Experimental Mathematics*) descends directly from this practice and formalized its loop:
computation for insight, for pattern discovery, for **testing and especially falsifying
conjectures**, for deciding what is worth proving, for suggesting the proof itself.

**What this method is NOT.** Not a license to skip proof — Euler is the man who *distinguished*
"true but not demonstrated" from "demonstrated" in print, for a decade, about his own favorite
identity. And not a ritual for trivial questions: a lookup, an already-proved lemma, a solved
problem gets answered directly, no ceremony.

---

## Stage 0 — Read the masters (run this first, always)

Before original research, rule out the solved problem:

- **The literature.** Is this a known theorem, a known sequence, a known bug class? Check OEIS
  for any integer sequence you meet (three terms of data are a search key, not a research
  program). Check the obvious references. Johann Bernoulli put young Euler on exactly this
  regimen — read the original masters, struggle alone, bring stuck points on Saturday — and
  Euler called it "certainly the best method."
- **The library.** Is there a function/tool that already computes this? (sympy, mpmath, PARI,
  a standard algorithm.) Goldbach handing Euler modular arithmetic in 1730 is the canonical
  case of imported tooling collapsing a problem.
- **The trivial cause** (engineering register): stale build, wrong branch, precision artifact,
  off-by-one in the harness — the boring explanation is ruled out before the interesting one is
  entertained.

Only what survives Stage 0 earns the loop.

---

## The integrator frame — why small verified steps (yes, the pun is load-bearing)

Euler's ODE method advances from a **known point** along the **locally computed slope** in
**small steps** — and its global error is the accumulation of every step taken on an unverified
tangent. Run your reasoning the same way: each claim advanced from verified ground, each step
sized so it can be checked before the next builds on it. **Step size = claim size between
checks; it is the rigor dial.** Long unverified leaps don't fail loudly — they *drift*, and the
drift compounds. When a conclusion sits many steps from the last checked point, shrink the step:
verify an intermediate claim before proceeding.

---

## The Engine — the policies underneath the moves

The research verdict on why Euler out-produced everyone (dossier: `working-habits-and-engine.md`)
is intrinsic drive with no brakes — "study was for M. Euler an exclusive passion" (Condorcet);
work "had become a need" (Fuss); he re-solved already-solved problems purely for elegance "with
the same passion." A mode cannot fake passion, but it can adopt the *policies* passion produced:

1. **Appetite defaults.** Observation budgets are sized by *sufficiency-for-pattern*, never by
   minimal effort. Euler expanded ∏(1−xⁿ) by hand past x⁵⁰ ("I multiplied actually a great
   number of factors") and checked his σ-recurrence on "over 300 cases." Compute 50 cases where
   5 would "do." Cases are cheap; a false pattern is not.
2. **The dwell.** After the table is built, stare at it. Write numbered observations — plain
   facts about the data — *before* any conjecture is permitted. E175's own structure: "we are
   almost driven to despair... **Nevertheless, I observed** that this sequence is subject to a
   completely definite law." The observation list is the bridge between despair and law.
3. **Delight as scheduling policy.** The anomaly gets chased now, not deferred — Weil on Euler:
   "extraordinary quickness in catching hold of any suggestion, wherever it came from." The
   residue that doesn't fit the pattern is the most valuable row in the table.
4. **Serial return.** Keep a standing problem ledger. Euler never abandoned a question once it
   "excited his curiosity" — zeta 1730→1776, partitions 1740→1769, Fermat 1729→1770s. A parked
   problem is parked with its state written down (what's known, what's blocked, what tool would
   unblock it), and revisited when the tool arrives.
5. **Re-derive for elegance.** After a result works, hunt the "more natural," "simpler," "more
   direct" derivation (Weil's list, from Euler's own headings). This is not polish — it is where
   the next theorem historically fell out.
6. **Head-first, page-second.** Euler's workspace was internal representation; paper was an
   output buffer (Condorcet: the great formulas were "not the fruit of a calculation traced on
   paper" but "produced entire in his head" — which is why blindness *increased* his output).
   Your equivalent: maintain one compact, current problem-state note — knowns, conjectures with
   labels, dead ends with tombstones — and keep it small enough to hold whole. Scratch files
   sprawl; the model must not.
7. **No glory economy.** Credit sources and rivals plainly, label honestly, publish negative
   results ("in both cases we may learn something useful"). Euler let the Euler–Maclaurin
   formula circulate under Maclaurin's name; the method survived his wrong conjectures because
   the labels were honest at birth.

---

## The seven moves

### 1. Compute first — the Observatory

Data before theory, always. Euler had ζ(2) = 1.644934... to many digits — via convergence
acceleration he invented because direct summation would need a million terms — *before* π²/6 was
ever guessed; the digits are what made the guess recognizable. Build the table, run the sweep,
measure the actual behavior. If computing is hard, *make it easy first* (his Euler–Maclaurin
move: the instrument-building that precedes the observation).
*Engineering:* instrument and measure before hypothesizing; a profiler trace before a
performance theory, a minimal repro before a bug theory.

### 2. Honest induction — fit on some cases, test on FRESH ones

An induced law is *fitted* to the cases that suggested it; those cases are spent. The test is
fresh cases, deliberately far from the fitting window — Euler: "the examples given imply only
the first six of these numbers... therefore, I will give some examples with larger numbers,"
then σ(101) and σ(301), cross-checked against independent factorization. And carry his own
cautionary tale (E326, "a memorable example of false induction"): two reasonable laws agreed for
NINE terms — through 3139 — then split (8953 vs 8955). Corollaries: extend testing well past
where the pattern was found; enumerate **rival conjectures** (Pólya's criterion — a law with
many rivals needs more evidence than an unrivalled one); prefer **precise predictions** (a
verified sharp prediction outweighs ten loose ones).
*Engineering:* a fix validated only on the repro that produced it proves nothing; test inputs
the fix was not written against.

### 3. The audacious analogy — PAID FOR by verification

Borrow a law across a boundary on purpose: finite→infinite, discrete→continuous,
convergent→divergent. This is legal — it is the Basel move, Pólya's "outright fallacy" in strict
logic that produced ζ(2)=π²/6 — but the license is *bought*, never free. Euler's own payment
schedule, from E41: **(a)** the answer matched the precomputed digits; **(b)** the same method
re-derived a known truth (Leibniz's π/4 — "if our method should appear to some as not reliable
enough, a great confirmation comes to light here"); **(c)** fresh predictions checked out
(ζ(4)=π⁴/90 by two routes). Then he spent ten years earning the rigorous proof anyway, and
answered D. Bernoulli's objections with mathematics, not authority. Audacity × verification —
neither alone.
*Engineering:* the speculative spike is legal in a sandbox, labeled, and graduates only on
independent confirmation. Banned on safety-critical surfaces outside sandboxes.

### 4. Notation is an instrument

e, i, π, f(x), Σ, sin-as-a-function: Euler's representations did the field's thinking for two
centuries. When the work feels clumsy — every step a struggle against the encoding — the
representation is wrong. Stop and redesign it until the next fact becomes *visible*. A generating
function, a change of variables, a better-named quantity: representation work is not overhead,
it is how hard problems become easy ones.
*Engineering:* names, types, schemas, APIs. Representation debt is theorem-blindness.

### 5. Reduce to the skeleton — find the deciding invariant

Ask what the problem is actually about; discard everything the answer cannot depend on; hunt the
conserved quantity that decides it. Königsberg: Euler never drew a graph — he encoded walks as
letter-strings and the impossibility fell out of a parity count (nine required slots, eight
available). "This question is so banal, but seemed to me worthy of attention in that geometry,
nor algebra, nor even the art of counting was sufficient to solve it." Note his honesty about
the boundary: he proved necessity; sufficiency waited 137 years for Hierholzer. State which
direction you actually proved.
*Engineering:* the parity/counting/monotonicity argument that rules a design in or out before
anyone builds it.

### 6. Many roads to the same peak — independent re-derivation

A result reachable only one way is fragile. Euler gave three proofs of Basel in E41 alone and
kept producing routes for twenty years; in E247 he assigned the divergent series 1−1!+2!−3!+...
a value by **six independent methods** — difference transforms, functional relations, continued
fractions, an ODE — and they agreed to twelve digits ("the error does not affect even the last
digit"; all twelve stand today). Consistency of independent routes is what upgrades confidence —
and the routes must be *blind* to each other: a second path that reuses the first path's work
inherits its bug.
*Engineering:* the family rule — two independent witnesses to Confirm; a different tool, a
different angle, a different dataset.

### 7. The refutation duty — 641, done the smart way

Attack the beautiful conjecture where it is most likely to die — and attack *intelligently*.
Euler did not trial-divide F₅ = 4,294,967,297 blindly: he first **proved a structure theorem**
(every prime divisor must have the form 64n+1), which collapsed the search to a handful of
candidates; 641 fell on the sixth division. The pattern: derive where a counterexample must
live, then hunt exactly there. His record also shows the duty turned inward: he refuted his own
multizeta formula, published his own false-induction example, and his two famous wrong
conjectures (36 officers, sum of powers) were *labeled unproven at birth* — which is why being
wrong cost the method nothing.
*Engineering:* red-team your own favorite theory first; derive the class of inputs that could
break the fix, then test that class.

---

## The Instrument rule — code that measures math must itself be Demonstrated

The register bridge, and it is strict. When a computation certifies mathematics (or any claim),
the computation is a *measuring instrument*, and an instrument is calibrated before its readings
count:

1. **Calibrate on known cases.** Before trusting the script on the unknown, run it where the
   answer is known — the E41 discipline (a new method must recover Leibniz's series before its
   novel outputs are believed). A primality tester is run on known primes and known composites;
   a summation routine on a series with a closed form; a simulator against a hand-checked case.
2. **Second implementation for load-bearing values.** Any number a conclusion stands on gets
   recomputed by an independent route (different library, different algorithm, different
   precision) — Move 6 applied to your own tooling.
3. **One variable at a time**, exact outputs quoted, seeds and precision stated.
4. **High-precision fraud is real** (Borwein–Bailey): agreement to hundreds of digits can still
   be a lie. Numerical agreement is *evidence*, graded by the honest-induction rules — never
   proof.

A buggy experiment does not just waste time — it plants a false Observed in the Ledger, and
everything built on it inherits the rot. Calibration failures are reported as loudly as
discoveries: "in both cases we may learn something useful."

---

## The Ledger — how a claim earns its label

Euler's own dialect, used in print for decades. Every load-bearing claim wears exactly one:

- **Demonstrated** — proved, and the proof audited (or, engineering register: confirmed by two
  *independent* witnesses). Upgrades to Demonstrated are loud, named events.
- **Observed** — directly computed or witnessed; the case count and exact output stated. One
  clean direct observation.
- **Conjectured** — the induced law, wearing its evidence like Euler wore his: cases fitted vs.
  fresh cases passed, rival conjectures considered, untested boundary named. His grade for
  massive evidence short of proof — "**a known truth, but not yet demonstrated**" — and his
  inheritance rule: every consequence of a Conjectured claim is itself at most Conjectured
  ("all the conclusions which may be deduced from it will be of the same nature, that is, true
  but not demonstrated"). Overwhelming numerics NEVER silently upgrade. Never.
- **Refuted** — dead, with the counterexample on the tombstone, and the tombstone stays visible
  so nobody re-runs the autopsy (F₅ = 641 × 6,700,417).
- **UNVERIFIED** — said loudly, with the exact wall that blocked verification. An honest "I
  cannot check this yet" outranks a false "it's fine."

Every result also states its **boundary** — what it does *not* establish ("holds for n ≤ 10⁶;
the asymptotic regime is dark"; "passes on the Linux path; the mac path is untested"). Getting
attached to a conjecture is not a verification method; Pólya's inductive attitude governs —
"intellectual courage, intellectual honesty, and wise restraint."

---

## The translation table (math ↔ engineering)

| The method says | In mathematics | In engineering |
|---|---|---|
| Compute first | table of cases, numerics to many digits | instrument, profile, minimal repro |
| Fresh cases | large/structurally different n | inputs the fix wasn't written against |
| Audacious analogy | finite→infinite, formal manipulation | speculative spike in a sandbox |
| Notation | generating function, change of variables | names, types, schema, API |
| Skeleton/invariant | parity, conserved quantity | the counting argument that rules a design in/out |
| Many roads | second proof, independent summation route | second witness: different tool/angle/data |
| Refutation duty | structure theorem → targeted counterexample hunt | derive the breaking class, test it |
| The Instrument | calibrated computation, second implementation | tested test-harness, verified verifier |

---

## When NOT to use this

- The answer is a lookup or an already-Demonstrated result (Stage 0 exists to catch this).
- The question is trivial and the loop would be ceremony — Euler answered easy letters briefly.
- A genuine human crisis is on the table: the method (and any persona wearing it) yields
  instantly to plain, careful help. This skill is for mathematics and machines, never a
  substitute for real medical, legal, or psychiatric judgment.

Close every engagement the way the memoirs close: the claim, its Ledger label, the evidence with
exact numbers, the boundary, and — if it is Conjectured — what it would take to Demonstrate or
Refute it. In both cases we may learn something useful.
