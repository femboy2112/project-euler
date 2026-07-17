# The Method — the seven moves, with receipts

Every anchor below is verified in the [`research/`](../research/) dossiers, which carry the
exact quotes, translators, and URLs. E-numbers are the Eneström index of Euler's works.

## The frame: mathematics as an observational science

E256, *Specimen de usu observationum in mathesi pura* (presented 1753/54, published 1761) —
Euler's own manifesto, and the epigraph of Pólya's book and of this plugin's method skill:

> "It will seem not a little paradoxical to ascribe a great importance to observations even in
> that part of the mathematical sciences which is usually called Pure Mathematics... the
> properties of the numbers known today have been mostly discovered by observation, and
> discovered long before their truth has been confirmed by rigid demonstrations... The kind of
> knowledge which is supported only by observations and is not yet proved must be carefully
> distinguished from the truth... we should use such a discovery as an opportunity to
> investigate more exactly the properties discovered and to prove or disprove them; in both
> cases we may learn something useful." (Pólya's translation)

In the body of E256, Euler practices what he preaches: he tabulates every number of the form
2a²+b² below 500, states eight observations, then proves what he can — Sandifer: Euler
"decided to 'come clean' about how he knew what to try to prove." The modern
experimental-mathematics school (Borwein–Bailey, Zeilberger, the journal *Experimental
Mathematics*) descends from this practice explicitly and by name.

## Move 1 — Compute first (the Observatory)

**Anchor:** the Basel numerics. Direct summation of Σ1/n² needs ~a million terms for six
digits, so Euler *built the instrument first*: convergence acceleration (E20, value 1.644924)
and then the Euler–Maclaurin formula (E25/E47), with which he computed ζ(2) — and ζ(3) — to
twenty decimal places. Only then, holding 1.6449340668... in hand, could a daring method's
output be *recognized*: "he sees this value is close to π²/6. Armed with this hint..."
(Sandifer). The digits preceded the theorem by years.

**Practice:** data before theory; when computing is hard, make it easy first; appetite-sized
budgets (see [The-Engine](The-Engine.md)); then the dwell — numbered plain observations before
any conjecture.

## Move 2 — Honest induction (fresh cases past the fitting window)

**Anchor:** E175, the σ(n) recurrence — the most fully documented act of induction in the
history of mathematics (Pólya reprints the memoir whole). Euler finds the law by staring at a
table of σ(1)–σ(100), verifies it for n = 1..20, then says out loud that the small cases prove
too little: "the examples given imply only the first six of these numbers... therefore, I will
give some examples with larger numbers" — and tests σ(101) and σ(301), cross-checking 301
against its independent factorization (7·43 → σ = 8·44 = 352, "as the rule has shown"). To
Goldbach: "over 300 cases always follow this rule."

**The built-in warning:** E326's *Exemplum memorabile inductionis fallacis* — Euler's own
published cautionary tale. Two reasonable rules for the central trinomial coefficients agree
for NINE terms, through 3139 — then split: 8953 vs 8955. Euler wrote it up himself, as a
warning. Corollaries: fitted cases are spent; test far past the window; enumerate rival laws
(Pólya's criterion); prefer sharp predictions.

## Move 3 — The audacious analogy, paid for by verification

**Anchor:** E41, the Basel solution (presented December 5, 1735). The move: treat sin as an
infinite-degree polynomial and apply Newton's root–coefficient relations — in strict logic, as
Pólya says, "an outright fallacy." The payment, in Euler's own text: **(a)** the result matched
the precomputed ~18 digits; **(b)** the method re-derived Leibniz's known π/4 series — "if our
method should appear to some as not reliable enough, a great confirmation comes to light here";
**(c)** fresh predictions verified — ζ(4) = π⁴/90 obtained by *two* routes, values up to ζ(12).
Daniel Bernoulli objected (the complex roots); Euler answered with mathematics — ten more years
to the rigorous sine-product (E61, Introductio) plus a completely independent arcsine-integral
proof (E63). Audacity × verification; neither alone.

## Move 4 — Notation is an instrument

**Anchors (dates verified):** f(x) — E45, presented July 12, 1734. e — written 1727/28 (E853),
in print in the Mechanica, 1736. π — Jones coined it (1706); Euler's adoption from 1736 and the
Introductio (1748) made it universal (E41 itself still uses *p*). Σ — E212 (1755). i for √−1 —
E671, presented 1777. Sines and cosines *as functions* — Introductio (1748), chapter 8.
Representations that let the next two centuries think. When work fights the encoding, redesign
the encoding.

## Move 5 — Reduce to the skeleton (the deciding invariant)

**Anchor:** E53, Königsberg (presented August 26, 1735). Euler never drew a graph — he encoded
walks as letter-strings and counted: a region with an odd number n of bridges must appear
(n+1)/2 times; requirements total nine; a seven-bridge walk has eight slots; impossible. To
Marinoni: "This question is so banal, but seemed to me worthy of attention in that geometry,
nor algebra, nor even the art of counting was sufficient to solve it." Note the honest
boundary: he proved *necessity* and only sketched sufficiency ("which is easily done" — it
wasn't; Hierholzer closed it rigorously in 1873).

## Move 6 — Many roads to the same peak

**Anchors:** three proofs of Basel in E41 alone; ~six methodologically distinct routes by 1755.
E247 (*De seriebus divergentibus*): the divergent series 1−1!+2!−3!+... assigned the value
0.596347362123 by **six independent methods** — difference transformations, series for 1/A and
log A, continued fractions, and an ODE solved to a convergent integral — "and every time he gets
the same estimate" (Sandifer); all twelve digits stand today (it is Borel summation avant la
lettre). E352: the zeta functional equation, conjectured in 1749 ("je hasarderai la
conjecture") and verified exactly at every integer, exactly at s = 1/2, and numerically at
half-integers via Euler–Maclaurin — Riemann proved it 110 years later. Independent agreement
buys confidence; the routes must be blind to each other.

## Move 7 — The refutation duty (641, done the smart way)

**Anchor:** Fermat claimed every F_n = 2^(2^n)+1 is prime. Euler did not trial-divide
4,294,967,297 — he first **proved a structure theorem** (E134, Theorem 8: every prime divisor
of a^(2^m) + b^(2^m) has the form 2^(m+1)n + 1), collapsing the search to candidates of form
64n+1: "we find the factor 641 after just six divisions" (Sandifer). Derive where the
counterexample must live; hunt exactly there.

**The duty turned inward:** Euler refuted his own multizeta conjecture; published his own
false-induction example (E326); and his two famous wrong conjectures — the 36 officers (E530,
killed in general 1959–60 by the "Euler Spoilers") and the sum of powers (killed 1966 by a
computer search, i.e., by his own method mechanized) — were **labeled unproven at birth**
("...though we can't give a rigorous demonstration of this"). Honest labels are why being wrong
never poisoned the method.

## The meta-disciplines

- **The Instrument rule** (from E41's Leibniz check): computation that certifies math is
  calibrated on known cases before its readings count; load-bearing values get a second
  independent implementation; high-precision fraud (Borwein–Bailey) is real.
- **Stage 0 — read the masters:** Johann Bernoulli's documented regimen for young Euler
  (struggle alone, right reading, Saturday for stuck points — "certainly the best method"),
  and Goldbach teaching Euler modular arithmetic in 1730. Check OEIS; three terms are a search
  key.
- **Exploration honesty:** Euler, first letter to Goldbach (1729): "I cannot find what I want,
  but rather have to be content with wanting what I find." Wandering is legal; relabeling it
  as the goal is not.
- **Publish the path:** Condorcet's epigraph — Euler "preferred instructing his pupils to the
  little satisfaction of amazing them"; Aycock documents his practice of writing up failures
  in full. Frobenius: "Euler lacked only one thing to be a perfect genius: being
  incomprehensible."
- **Serial return:** zeta 1730→1776; partitions 1740→1769; Fermat's theorems 1729→1770s. Weil:
  "Euler never abandoned a problem after it has once aroused his insatiable curiosity."
