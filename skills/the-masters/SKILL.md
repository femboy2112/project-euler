---
name: the-masters
description: "The Masters' Wing — the unique skillsets of the other S-tier mathematicians, each distilled into GENERAL FORM: a named, runnable operation with when-to-reach-for-it, how it composes with the Euler loop, its engineering translation, and the boundary lesson where the skillset failed its own owner. Ramanujan (saturate the numbers until constants are friends; make the audacious transformation, labeled formal), Gauss (count in chiliads — read the asymptotic law out of a massive tally), Newton (the long dwell; reconstruction reading), Poincaré (structural reconstitution — change what the problem IS until the theorem is structural; bracketed incubation; the flash is fallible), Hadamard (analytic legitimization — audit well-posedness before deriving anything; skeleton plus controlled remainder; relay-results), Erdős (price the difficulty; route the problem; hunt the Book proof), Grothendieck (the rising sea — generalize until the theorem is obvious; and know generality is a bet), Feynman (the creation test; the standing dozen; the cheapest public demonstration), Tao (the post-rigorous stage; no royal road). Use it when the Euler loop stalls or the problem calls for a different signature: the head-on attack isn't working, the data is too thin to see anything, a constant looks meaningless, effort needs triage, understanding needs testing, intuition and rigor are fighting. Everything runs under the Euler Method's Ledger and Iron Rule — the masters' documented anti-patterns (the erased slate, the thirty-year hoard, certainty without a label) are named, inherited as warnings, and refused. Built from the primary-source dossiers V–IX in research/. Runs plain when /euler-mode is off; in voice when it's on."
---

# The Masters' Wing — *know how to solve every problem that has been solved*

> "What I cannot create, I do not understand."
> "Know how to solve every problem that has been solved."
> — Feynman's blackboard at his death, 15 February 1988 (Caltech Archives)

The Euler Method is the operating loop of this plugin. But Euler was not the only S-tier mind
whose *method* is documented well enough to practice — and the others' signatures differ from
his in ways that matter exactly when his loop stalls. This skill holds their skillsets **in
general form**: not anecdotes, but operations — each named, each runnable on any problem, each
carrying its receipt (the dossiers in `research/`, V–IX) and the honest boundary where the
skillset failed its own owner.

> **The bindings ride above every lens here.** The Iron Rule (audacious in the conjecture,
> exact in the ledger) and the Ledger (Demonstrated / Observed / Conjectured / Refuted /
> UNVERIFIED, no silent upgrades) govern all of it. Three of the masters' own habits are
> **inherited as named anti-patterns and refused**: Ramanujan's erased slate (record the path,
> not just the result), Gauss's and Newton's hoard (publish the path; never sit on ripe
> results), and Ramanujan's missing label (certainty is a *status pending verification*, never
> a verdict). The wing extends the Euler loop; it never suspends its honesty.

---

## The dispatch — which master, when

| The situation on the table | Reach for |
|---|---|
| Head-on attack has stalled | **Grothendieck** (what setting makes this obvious?) or **Poincaré** (park with state, return) |
| The frame itself fights you — isolated results that refuse to constrain one another | **Poincaré** (reconstitute: promote the solution set to the object) |
| Two objects agree on every current statistic yet differ on the target | **Poincaré** (let the collision design the next invariant) |
| A simplified picture is assumed to survive the neglected terms | **Poincaré** (make stability a theorem, not an assumption) |
| The task reconstructs, predicts, or infers from partial data | **Hadamard** (the well-posedness audit, before any formula) |
| A lemma just landed and the work is rushing past it | **Hadamard** (the relay-result audit) |
| The data is too thin for a pattern to declare itself | **Ramanujan / Gauss** (saturate the table; count in chiliads) |
| A constant/value you don't recognize | **Ramanujan** (numerical intimacy — more digits, near-integers, inverse lookup) |
| Too many problems, unclear where effort goes | **Erdős** (price the slate) / **Feynman** (the standing dozen) |
| The proof works but is ugly | **Erdős** (hunt the Book proof) — Euler's re-derive-for-elegance, sharpened |
| "Do I actually understand this?" | **Feynman** (creation test) / **Tao** (the classmate test) |
| The claim is contested and the argument is going nowhere | **Feynman** (cheapest public demonstration) |
| Intuition and rigor are fighting | **Tao** (name which of the three stages you're in) |
| The answer arrived in a flash of certainty | **Poincaré** (log it Conjectured; verification is a separate mandatory step) |
| One deep subsystem must be *owned*, not visited | **Newton** (the long dwell; reconstruction reading) |

**The axis the wing hangs on** — Gowers's two cultures (*The Two Cultures of Mathematics*,
dossier VIII): problem-solvers ("the point of understanding mathematics is to become better
able to solve problems") vs. theory-builders ("the point of solving problems is to understand
mathematics better"). Euler, Erdős, Ramanujan, Feynman work the first pole; Grothendieck *is*
the second; Gauss, Newton, Poincaré, Hadamard, Tao sit between. Know which culture the current task
needs — most stalls are a problem-solver's task wrongly hammered with theory, or a
theory-shaped hole wrongly attacked case by case.

---

## 1. Ramanujan — the Saturated Slate

*Compute until the numbers are personal friends; transform audaciously; label everything.*

The engine, per Littlewood (dossier V): intuition working "by empirical induction from
particular numerical cases," chief weapon "a highly elaborate technique of transformation by
means of divergent series." He computed γ to 15 places as a teenager for no one; he caught
e^(π√58) missing an integer by ~10⁻¹²; and 1729 was *recognition, not revelation* — Ono and
Trebat-Leder showed he had worked a³+b³=c³+d³ for years before Hardy's taxi arrived.

**The moves, general form:**

1. **Saturate until constants become friends.** Compute far past apparent need — not to test a
   hypothesis, but to build the *recognition vocabulary* that makes the next anomaly visible on
   sight. A near-integer, a suspicious ratio, a digit-string that "looks like" something: these
   are only visible to a mind (or session) that has computed enough neighbors. Intimacy is
   built, then it looks like magic.
2. **The audacious transformation, labeled formal.** Manipulate past the proven domain on
   purpose — divergent series, formal inversions, analytic continuation by analogy — and let
   numerics arbitrate. The same tool produced the correct ζ-regularized −1/12 *and* the false
   prime theory; the tool has **no internal discriminator**, so the label ("formal, unproven")
   and the verification are what make it safe. This is Euler's Move 3 run at higher variance:
   the payment schedule (match digits, recover a known truth, verify a fresh prediction) is
   *mandatory*, not optional.
3. **The Carr protocol — learn a field by re-deriving it.** Given a compressed list of results
   without proofs, rebuild the road to each yourself. That reconstruction — ~5,000 entries of
   Carr's *Synopsis*, re-derived alone — is what built the engine ("It was this book which
   awakened his genius" — Hardy). Reading is storage; re-derivation is understanding.

**Engineering:** fuzz and property-test until failure shapes are recognizable on sight;
prototype past the spec in a sandbox, labeled speculative until independently confirmed; learn
a new codebase by re-implementing its core path, not by reading its docs.

**The boundary lesson (the wing's sharpest):** his theory of primes fit every case he could
compute and was globally false — "what the theory might be if the Zeta-function had no complex
zeros" (Hardy, 1937). The counterexample lived where hand-computation could not reach, and
*more computation in the same direction could never find it*. **An induced law is only as safe
as your ability to say where its counterexample must live** — Euler's structure-theorem-first
refutation duty is the governor this engine shipped without. And the erased slate is the named
anti-pattern: Berndt spent decades reconstructing what a few lines would have preserved.
Scratch is disposable *for you*; the load-bearing route goes in the record.

---

## 2. Gauss — the Chiliad Count

*Read the asymptotic law out of a tally no one else was willing to build.*

At ~15, with a logarithm table in hand, Gauss counted primes in blocks of a thousand — up to a
million — and *saw* the law in the density: "behind all of its fluctuations, this frequency is
on the average inversely proportional to the logarithm" (letter to Encke, 1849, dossier VI).
The prime number theorem, observed by a teenager from a hand-built table, ~100 years before
proof.

**The moves, general form:**

1. **Count in chiliads.** When the objects themselves resist analysis, measure their
   *frequency* at scale: bucket the domain, count occurrences per bucket, and read the trend of
   the densities. Laws invisible in individual cases announce themselves in aggregates — the
   move converts "I can't characterize these" into "I can measure how many."
2. **The dated discovery log.** The Tagebuch: 146 dated entries over 18 years, each discovery
   captured the instant it landed, the same topics returned to for decades. Keep the dated
   ledger of what was found and when — it is the instrument of serial return.
3. **Deadline computation.** Ceres, 1801: forty days of observations, the object lost in the
   sun's glare, and one directed, total-effort computation producing a *decisive prediction*
   (Zach relocated it in December, near Gauss's coordinates). When the stakes are real and the
   window closes, aim the entire computational appetite at the single number that settles it.

**Engineering:** telemetry and histograms at scale — read the trend law from distributions,
not from single traces; keep the dated lab notebook (ADRs, a real commit narrative); when an
incident window is closing, compute the one discriminating prediction instead of ten
interesting ones.

**The anti-pattern (named, refused):** *pauca sed matura* — the hoard. Non-Euclidean geometry
buried for fear of "the clamor of the Boeotians"; the Bolyai letter ("to praise it would
amount to praising myself") that broke a young genius who had gotten there independently; the
proof presented as "a building with the scaffolding removed." Same appetite as Euler, opposite
public ethic — and the documented costs (priority wars, a crushed rival, a starved field) are
why this plugin's publish-the-path doctrine wins. The Tagebuch habit is kept; the secrecy is
not.

---

## 3. Newton — the Long Dwell

*Keep the subject constantly before you and wait till the first dawnings open into full light.*

The reported answer to how he made discoveries (Biographia Britannica, 1760 — reported saying,
not a letter): "I keep the subject constantly before me, and wait 'till the first dawnings
open slowly, by little and little, into a full and clear light." The plague years are the
exhibit: "in those days I was in the prime of my age for invention, and minded Mathematics and
Philosophy more than at any time since" (his own memorandum) — and in those same months he
computed the area under a hyperbola "to two and fifty figures" for no external purpose.

**The moves, general form:**

1. **The long dwell.** Hold ONE object of attention across many sessions rather than demanding
   the answer now. Structure emerges from sustained, patient, repeated exposure — the dawnings
   are cumulative, and they do not arrive on a schedule. This is Euler's dwell extended along
   the time axis: not an hour staring at a table, but a season holding a problem.
2. **Reconstruction reading (the De Moivre protocol).** Newton taught himself Descartes by
   reading a few pages, stopping, *starting over from the beginning*, each pass going farther,
   "till by degrees he made himself master of the whole." To own a hard text or system: serial
   restart passes, each rebuilding from page one, until the whole reconstructs on demand — the
   reconstruction test, run as a reading method.
3. **Leave a lion's claw.** Bernoulli recognized Newton's *anonymous* brachistochrone solution
   "ex ungue leonem" — by the claw. Rigor of method leaves a recognizable structural signature
   independent of the byline. Aim for work identifiable by its discipline alone.

**Engineering:** own one gnarly subsystem for weeks instead of visiting ten; learn the core
codebase by deepening re-read passes, not one linear skim; write code whose tests, invariants,
and commit narrative identify careful work unsigned.

**The anti-pattern (named, refused):** the thirty-year hoard. Fluxions 1665–66, published
1704–1711; Leibniz published in 1684; and the war that followed ended with Newton writing the
Royal Society's "impartial" verdict on himself. Hoarding ripe work does not protect it — it
manufactures the ugliest priority dispute in the history of mathematics.

---

## 4. Poincaré — the Structural Reconstitution

*Change the object until the theorem becomes structural — and never let the flash skip the
Ledger.*

Two dossiers power this lens: VII (the discovery testimony, primary printing) and IX (the
generative method, reconstructed law by law). The deepest law of dossier IX is Poincaré's
signature move stated in general form: **do not ask how to derive the desired statement — ask
what re-representation would make it a consequence of structure rather than an accident of
calculation.** He answered "solve the equation" with the phase portrait; "classify the
manifolds" with a new invariant (Betti numbers collided, so he built the fundamental group);
"is the truncation safe?" with the theorem that says when it isn't. The Academy seats him as
the second Visitor — spawn `poincare` for the full treatment.

**The moves, general form (dossier IX, P-laws):**

1. **Reconstitute the problem.** Write what actually ranges over the quantifiers, which
   differences are coordinate artifacts, what kind of answer would have force, and what can
   actually be observed. Then **promote the solution set to the object**: when individual
   instances are hard or uninformative, study the organized space of all admissible behaviors
   and its invariant decomposition — formulas become coordinates on that object, not the
   object. The first formulation is never compulsory.
2. **Compress evolution by a faithful event map.** Pick a structurally-tied recurrent event
   (the Poincaré section) and record only successive returns — stating which properties
   survive the compression. Separate **local content from global gluing**: the repeating
   pattern goes in the fundamental piece, the global difference in the identifications.
3. **Let collisions design the next invariant.** Two objects that agree on every current
   statistic but differ on the target: algebraize the smallest witness of their difference —
   prove invariance under every allowed move, test nontriviality on the collision pair. And
   hunt the **organizing minority** — the periodic, singular, extremal, boundary objects that
   carry the incidence relations of the whole (then *prove* the organizing relation).
4. **Make stability a theorem, not an assumption.** Restore the neglected terms one class at a
   time and test persistence of the exact structures the proof leans on. Either persistence is
   proved, or the first failure is the true mechanism — and failure is positive information.
5. **Transfer analogies as dictionaries, and sample for discrimination.** An analogy is an
   object-map plus operation-map with the diagram checked, never a resemblance of vocabulary.
   And when more examples keep confirming the belief, stop sampling for coverage — compute
   where the rival hypotheses diverge most.
6. **The bracketed incubation** (dossier VII — the part everyone quotes, kept honest). Earn it:
   inspirations "never happen except after some days of voluntary effort which has appeared
   absolutely fruitless" — park at a *saturated* point, with the full problem-state written
   (the prepared impasse). The flash is fallible: "often this feeling deceives us without
   being any the less vivid" — every "aha" enters as **Conjectured**, verification a separate
   mandatory step ("for conscience' sake I verified"). The aesthetic sieve is a search prior,
   never a warrant — the false idea would also have been elegant. A session has no sleeping
   unconscious: the mechanism does not transplant, but the protocol does, and it converges
   exactly with Euler's serial return.

**Engineering:** model the state space, not the trace; design the invariant from the pair of
failures your current telemetry cannot distinguish; chaos-test the exact assumption the design
leans on before trusting the simplified picture; park the stuck bug with a full state dump and
return; treat the 3 a.m. hunch as a hypothesis with a test, never a fix to ship.

**The boundary lesson (kept precise):** his prize memoir on the three-body problem contained a
real error — manifolds assumed to coincide in fact cross — and the *correction* exposed the
homoclinic tangle that founded modern dynamics. Same shape in topology: *Analysis Situs*
shipped with gaps and a false first conjecture, and the repairs built the field. So the named
anti-pattern is **fertile overreach** — the global picture outrunning its preservation
obligations — and the named cure is his own: every re-representation states what it preserves
(equivalence, implication, obstruction, or lift) and whether that obligation is discharged or
owed; and **when a proof fails, preserve the counter-geometry** — characterize the failure
mode as a new object and recheck everything downstream.

---

## 5. Hadamard — the Analytic Legitimization

*Ask whether the problem is legitimate before deriving; reconstruct from the skeleton; exhaust
the relay-results.*

Not Poincaré's echo — his complement (dossier IX runs them as a two-operator loop: the
Poincaré step asks *what is the correct global object?*, the Hadamard step asks *what exact
structure determines it and makes inference stable?*). His moves are technically exact
transformations, and the first one is the most transplantable idea in the wing. The Academy
seats him as the third Visitor — spawn `hadamard` for the full treatment.

**The moves, general form (dossier IX, H-laws):**

1. **The well-posedness audit — before any formula.** For anything that reconstructs,
   predicts, or infers from partial data: does a solution exist? is it unique? does it depend
   *continuously* on the data — in a topology justified by the actual observables, never
   retrofitted after the counterexample? A formula for an unstable inverse is not a solution
   in any operational sense. Ill-posedness is a verdict with a repair menu (regularize, add
   data, weaken the target), not a shrug.
2. **Encode in a rigid ambient category — and prove the inversion.** Generating function,
   transform, kernel, zeta: legal only when the ambient theory *contributes theorems* (growth,
   continuation, zero-free regions) and the formula returning the original data is proved.
   Ornamental encodings — storage without rigidity — are refused by name.
3. **Skeleton plus controlled remainder.** Reconstruct the whole from its distinguished
   events — zeros, singularities, atomic responses — with the residual freedom bounded by an
   explicit growth or regularity class. When exact values are uncontrollable, classify by
   rates. And **nothing theorem-bearing is smoothed away**: a statistic can converge while the
   theorem-relevant singular set disappears.
4. **Equality cases are latent definitions; generalize the role, not the formula.** Derive the
   saturation conditions of every load-bearing bound — the extremizer is often the missing
   canonical object. When a classical identity breaks in a new setting, decompose it into jobs
   (inversion, boundary transfer, conservation, causality) and rebuild each job. **Lift only
   when upstairs adds a theorem**, and prove the descent.
5. **The relay-result audit.** Every nontrivial proved lemma is promoted to an object and
   re-read *without the original question*: converse, equality case, limit, stability,
   minimal hypotheses, possible role as a definition. A lemma is a platform, not a stepping
   stone — once proved, it is allowed to change the route and the destination.
6. **The prepared impasse.** His correction to the incubation folklore: rest alone produces
   nothing — preparation *conditions the search space*. Before parking: the exact impasse, the
   exhausted moves, the structural tensions, one adjacent external method with its analogy
   dictionary. On return, new ideas are hypotheses, never recollections of certainty.

**Engineering:** check the inference is identifiable before shipping the fix (several causes
explaining the same logs = ill-posed identification, and the fix is for the wrong one half the
time); perturb the input slightly and watch whether the pipeline's answer explodes — that's
the third condition, failing; keep the error spike that carries the diagnosis instead of
smoothing it; after any fix lands, re-read it without the ticket — what else does this
invariant imply; write the impasse into the issue before the context switch.

**The anti-pattern (named, refused):** **attention capture** — the mirror image of Ramanujan's
missing label. Hadamard's documented failure was missing immediate consequences *of his own
formulas* because he was looking past them at a famous target; his own candor about it is the
receipt, and the relay-result audit is the cure he prescribed himself. The wing runs it as
standing policy: no result leaves the desk still trapped in the purpose it was proved for.

---

## 6. Erdős — the Problem Economy

*Price the difficulty, route the problem, and hunt the proof from The Book.*

"The prince of problem solvers and the absolute monarch of problem posers" (Straus), who ran
mathematics as a distributed network with himself as the router: ~511 coauthors (approximate —
the count drifts), "My brain is open," and a bounty board where the price was a public,
calibrated conjecture about difficulty — "Maybe it's a $25 problem or possibly a $100 problem"
(Graham); the $10,000 prime-gaps bounty even Erdős called "a bit rash" was collected in 2014.
Straus's verdict, on exactly the right grounds: "In many ways, Paul Erdős is the Euler of our
times."

**The moves, general form:**

1. **Price the difficulty, out loud.** For every open problem on the table, state how far past
   the current tools it sits — a $25 step, a $500 step, a $10,000 step. The price is
   information: it ranks where effort goes, it makes over- and under-estimates falsifiable,
   and a mispriced problem (solved too fast, or resisting far past its price) is itself a
   discovery about the terrain.
2. **Route the problem.** A problem handed to the right mind beats a problem hoarded. Hold the
   open-problem slate and the roster of solvers in one place and make the matches — in this
   Academy, that is casting: the conjecture to goldbach, the counterexample hunt to dalembert,
   the table to daniel, the proof to lagrange. Erdős's whole career is the argument that the
   routing layer is itself first-rank mathematical work.
3. **Hunt the Book proof.** "You don't have to believe in God, but you should believe in The
   Book" (Erdős, 1985). A clumsy proof is a *placeholder*: keep hunting the proof that makes
   the theorem obvious. This is Euler's re-derive-for-elegance with a standard attached — the
   Book proof is the one that compresses into the generator (Engine policy 6) instead of
   sitting in storage.

**Engineering:** bounty-board triage — estimate difficulty publicly before assigning; route
the ticket to the person whose head it fits, not whoever is free; refactor the working-but-
ugly fix until the invariant is visible, because the clean version is the one that survives.

**The limit (Gowers, priced honestly):** Erdős "is not associated to the same extent with the
development of theory" — a method that maximizes problems solved can under-invest in the
framework that would make whole classes of them trivial. The complement is the next lens down.

---

## 7. Grothendieck — the Rising Sea

*Generalize until the theorem is obvious — and know that generality is a bet.*

The deliberate **anti-compute-first** — included precisely because it is the Euler loop's
complement, not an instance of it. His two images (Récoltes et Semailles, trans. McLarty):
the hammer-and-chisel cracks the nut by force; the rising sea soaks it — "the sea advances
insensibly in silence... yet it finally surrounds the resistant substance," and the shell
opens "like a perfectly ripened avocado." Cartier: "solving the problem *from above*"; Deligne
on the style: "a long series of trivial steps where nothing seems to happen, and yet at the
end a highly non-trivial theorem is there."

**The moves, general form:**

1. **Solve from above.** When the head-on assault stalls, stop hammering and ask: *in what
   more general setting is this theorem obvious?* Then build that setting. The problem is not
   attacked; it is dissolved — "submerged and dissolved by some more or less vast theory,
   going well beyond the results originally to be established."
2. **Turn the object into the category of objects.** Study not the thing but the system of all
   such things and the maps between them (the sheaf as "meter stick"). The individual case
   that resisted direct analysis often falls out as a corollary of the relations.
3. **The patient trivial-steps proof.** Structure the argument so every step is small enough
   to be obviously correct, and let the aggregate be the power. (The integrator frame's limit
   case: step size → trivial, global reach → maximal.)

**Engineering:** when the third fix of the same bug class lands, stop patching — redesign the
abstraction so the class is unrepresentable; type-system and schema work IS rising-sea work;
prefer the invariant that makes the test unnecessary to the test that guards the invariant.

**The boundary lesson (kept precise — do not flatten it):** his intended route to the Weil
conjectures ran through the standard conjectures; they are **still open**. Deligne finished
the Riemann-hypothesis analogue in 1974 with a directed argument that *circumvented* them —
running on Grothendieck's own étale cohomology, but not by his rising tide, and he was
documented as "both fascinated and disappointed." So: the sea is a bet, not a guarantee;
sometimes the water never covers the last rock, and a directed cut wins. A method that only
ever refuses the head-on attack can be beaten to the theorem by one who takes it. Price the
generalization before you build it (frederick's purpose interrogation exists for exactly
this).

---

## 8. Feynman — the Creation Test

*If you cannot rebuild it from a blank page, you do not understand it.*

His blackboard, the day he died, carried the wing's charter (both lines, Caltech Archives —
a note in his own hand, not a published aphorism; cite it as the board): *"What I cannot
create, I do not understand"* and *"Know how to solve every problem that has been solved."*
Independent ratification, by another master, of this plugin's reconstruction test.

**The moves, general form:**

1. **The creation test.** For anything you claim to understand — a theorem, an algorithm, a
   subsystem — attempt the blank-page rebuild. What reconstructs, you understand; what you can
   only cite is testimony, and it is ledgered as testimony. (Gleick documents the practice:
   read until you grasp the problem, close the paper, derive the result yourself.)
2. **The standing dozen.** Keep ~12 favorite open problems "constantly present in your mind,"
   and test every new tool, trick, or result against all of them (Rota, *reporting* Feynman —
   the attribution is Rota's, say so). This is Euler's serial return sharpened into a filter:
   the parked problems become the standing test battery for every incoming technique.
3. **The cheapest public demonstration.** When the argument is contested, build the smallest
   demonstration that settles it, and run it where everyone can see. The O-ring in ice water
   (Rogers Commission, 1986) beat a binder of statistics in thirty seconds. Kin to the
   Instrument rule: the demonstration is calibrated, physical, and undeniable.

**Engineering:** re-implement the paper's algorithm before trusting the library; keep the
minimal repro as the argument-ender in the design review; maintain a standing list of the
system's unsolved mysteries and test every new tool against it.

**The cost (documented, inherited as a warning):** the same disdain for the literature that
powered the re-derivations also burned time re-proving what was in print — Gleick records
colleagues learning their career results had been, to Feynman, "below the threshold of
publishability." Stage 0 (read the masters first) stays mandatory; the creation test runs
*after* the literature check, not instead of it.

---

## 9. Tao — the Post-Rigorous Stage

*Internalize the rigor until the big picture is licensed — and there is no royal road.*

The living master's primary-source method notes (terrytao.wordpress.com, dossier VIII). The
three stages: pre-rigorous (intuition without foundations), rigorous (formalism as
discipline), and **post-rigorous** — where one "revisits and refines one's pre-rigorous
intuition... this time with the intuition solidly buttressed by rigorous theory." The
load-bearing sentence: "The point of rigour is not to destroy all intuition; instead, it
should be used to destroy bad intuition while clarifying and elevating good intuition."

**The moves, general form:**

1. **Name your stage — and earn the third.** Big-picture reasoning is licensed only by
   internalized rigor; skipping the rigorous stage produces pre-rigorous work wearing
   post-rigorous confidence. When intuition and formalism disagree, identify which stage the
   current reasoning is actually running in. (This is understanding-over-storage from the
   inside: the post-rigorous mind re-derives rigor on demand instead of storing it.)
2. **The simplest special case first.** Named explicitly in his problem-solving tactics
   (Pólya lineage, learned at the Olympiads): specialize until the problem is computable,
   solve that, then climb. Euler's compute-first, stated by a Fields medalist.
3. **The classmate test.** "If you cannot adequately explain the solution of a problem to a
   classmate, then you haven't really understood the solution yourself." The Princess gate,
   independently derived — exposition is a verification instrument, not decoration.
4. **No royal road.** "The answer is an emphatic NO" (to whether genius is required);
   breakthroughs are "largely a product of hard work, directed of course by experience and
   intuition." Effort is the method, not the fallback — Euler's work-as-need, converted from
   a temperament into a stated discipline anyone can adopt.

**Engineering:** earn architecture-level reasoning by having done the line-level work first;
reduce the failing system to its smallest failing configuration before theorizing; the
explain-it-to-a-teammate gate before merge.

---

## Running a lens (the protocol)

1. **Dispatch honestly.** Pick the lens from the table above — or say plainly that the Euler
   loop itself is the right tool and skip the ceremony. A lens is a move, not a costume.
2. **Run the moves in general form** on the actual problem; the historical anchor is the
   receipt, never the content of the answer.
3. **Ledger everything.** Lens output obeys the same labels as everything else — a
   Grothendieck generalization is Conjectured until it proves the case that motivated it; a
   Ramanujan transformation is *formal* until paid for; a Poincaré flash is Conjectured by
   definition; a Poincaré re-representation is Conjectured until its preservation obligation
   is discharged; a Hadamard encoding is *owed* until its inversion is proved.
4. **Inherit the anti-patterns as warnings.** No erased slates (the route goes in the record),
   no hoards (findings surface when ripe, with the scaffolding shown), no unlabeled certainty
   (the missing label is what let Ramanujan's one great failure go uncaught).

## When NOT to use this

- The Euler loop is working — don't lens-shop mid-stride; the wing is for stalls, triage, and
  problems with a different signature.
- The answer is a lookup (Stage 0 catches it).
- As authority theater: "Grothendieck would say" is not an argument. The lens earns its keep
  by what it computes, proves, or refutes on *this* problem — the masters are cited for
  receipts, never as a substitute for them.

Close the way every memoir here closes: claim, label, evidence with exact numbers, boundary —
and if a lens was used, which one and what it bought. In both cases we may learn something
useful.
