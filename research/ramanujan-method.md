# Dossier V — Ramanujan's Working Method and Causal Engine

> Research dossier for Project EULER (masters' wing), compiled 2026-07-16 by a web-research agent.
> Figure: **Srinivasa Ramanujan** (1887–1920). Scope: the METHOD — what he *did*, slate and
> notebook; the causal engine behind the output; the moves transplantable to a modern working
> session; and where the method FAILED for lack of a discipline Euler had. Not a biography, not a
> results catalog.
> Labels: **VERBATIM** (exact wording read from source), **PARAPHRASE** (content confirmed,
> wording condensed), **LEGEND-UNVERIFIED** (circulates widely, primary attestation not traced).
> This file is a receipt: the plugin quotes from it and must not upgrade any label.

**Scope note on sources.** No live eyewitness document survives the way Fuss/Condorcet do for Euler —
Ramanujan's tragedy is precisely that the *path* was erased. The primary witnesses are **G.H. Hardy**
(1921 LMS obituary; 1937 *American Mathematical Monthly* essay "The Indian Mathematician Ramanujan";
1940 *Twelve Lectures*; worked beside him 1914–1919) and **J.E. Littlewood** (*Miscellany*). The modern
reconstructive authority is **Bruce Berndt** (*Ramanujan's Notebooks* I–V; the 2012 lost-notebook oral
history). Read in full this session: MacTutor, the Bhāvanā essay on lost work, Wolfram's "Who Was Ramanujan?",
Wikiquote (sourced page numbers), Alladi's Inference essay, the Baez/Azimuth taxicab post, the IITK
book-excerpt of *Twelve Lectures*. Two arXiv PDFs (oral history 1208.2694; "Thoughts from God" 1707.03379)
returned un-parseable binary and were used only via search snippets — flagged where load-bearing.

---

## 1. The instrument: the slate, the notebook, and the erased path

The physical workflow is the single most important — and most costly — fact about how Ramanujan worked.

**The slate-and-transfer loop — PARAPHRASE (Berndt, via Wikipedia and Bhāvanā):** He did most of his work,
and most of what proofs he had, *on a slate* — chalk on stone — because paper was expensive and he was
poor. He worked a problem, erased the intermediate calculation with his elbow, and transferred only the
*final result* to a hardbound notebook. Slates were standard for Madras students; paper was a luxury.
(Wikipedia cites Berndt: "did most of his work and perhaps his proofs on slate," then "transferred the
final results to paper.")

**The erasure, imaged — VERBATIM (Bhāvanā essay, photo caption):**
> "the slate on which Ramanujan scribbled his thoughts, if only to frantically erase them with his
> elbow, and then quickly refill it all over again with some more calculations."

**What survived — PARAPHRASE (Berndt):** three main notebooks holding roughly **3,000–3,900 results,
almost all without proof**; a first letter carrying ~120 theorems (Berndt counted 67 in surviving pages);
and the "lost notebook" of his final year, rediscovered by **George Andrews in 1976** in Trinity's Wren
Library. Of the Cambridge conversations with Hardy — where the *reasoning* lived — Berndt's verdict is
stark: **VERBATIM (oral history, via search snippet):** "we have no records at all of any of these
conversations." Because the derivations were erased, later mathematicians could neither easily verify nor
extend the work; Berndt's own *decades* went into reverse-engineering proofs from bare statements — the
exact inverse of the Euler archive, where the path is the artifact.

> **Boundary lesson (developed in §7, §9):** Ramanujan optimized for the *result* and treated the
> *derivation* as disposable scratch; Euler optimized for the *path* and published it, false starts
> included. Same computational appetite; opposite storage policy. The erased slate is the anti-pattern
> the plugin's "understanding over storage / reconstruction test" exists to keep from turning *lossy*.

---

## 2. Carr's *Synopsis* — compression that forced reconstruction

**The book — PARAPHRASE (MacTutor, Wikipedia):** around age 16 Ramanujan obtained **G.S. Carr's *A
Synopsis of Elementary Results in Pure and Applied Mathematics*** (1886): ~**5,000 theorems and formulae,
terse and mostly *without* proofs**, plus a dated index to European journals. It was his primary
mathematical education, and he worked through it by **deriving each result himself** — the book gave the
*destination*, he reconstructed the *road*. Hardy — **VERBATIM (*Twelve Lectures*, via IITK):** "It was
this book which awakened his genius"; "there is no doubt that it influenced him profoundly." MacTutor
notes the downside — **VERBATIM:** "the style of the book was to have a rather unfortunate effect on the
way Ramanujan was later to write down mathematics" (terse, result-only — literally the format of the 1913
letter).

> **Euler-connection (genuine): the reconstruction test.** Carr is the historical exhibit for the
> *understanding-over-storage* doctrine: a stored list of results is worthless until you can *re-derive*
> it, and the re-derivation is what built the instrument in Ramanujan's head. **But the same episode
> warns:** he never externalized the skill — he could regenerate a result on demand but did not record
> *how*, so it died with him. Storage-free understanding is a personal superpower and an institutional
> catastrophe.

---

## 3. The method itself: compute, observe, induce

Every serious witness describes the same engine — numerical experiment first, pattern-spotting, then a
bold induced law — nearly identical in *shape* to the Euler loop, minus the verification stage.

**Hardy's summary of the whole method — VERBATIM (Hardy, on Ramanujan's mode of discovery; wording
confirmed across Wikipedia and multiple secondary sources, original page not personally opened this
session):**
> "[arrived at] by a process of mingled argument, intuition, and induction, of which he was entirely
> unable to give any coherent account."

**Littlewood on the mechanism — VERBATIM (Littlewood, *Miscellany*, via Wikiquote, pp. 95–97):**
> "his intuition worked in analogies, sometimes remote, and to an astonishing extent by empirical
> induction from particular numerical cases."

**Littlewood on his chief tool — VERBATIM (same source):**
> "his most important weapon seems to have been a highly elaborate technique of transformation by means
> of divergent series."

**The experimental-mathematics reading — PARAPHRASE/VERBATIM (Wolfram):** he was "an experimental
mathematician: going out into the universe of mathematical possibilities and doing calculations to find
interesting and significant facts." **Approximations were routinely part of the process even when the
final result was exact** — he computed e^(π√58) ≈ 262537412640768743.99999999999925…, *noticed* the
near-integer, and built theory outward from it. Compute-first, dwell, induce — the Euler opening move at
superhuman speed. His own statement of numerical trust — **VERBATIM (to Hardy, via Wolfram):** "For my
results are verified to be true even though I may take my stand upon slender basis." And by 1904 he was
computing **γ to 15 decimals** and rediscovering the Bernoulli numbers unprompted — the tables-and-tables
Euler appetite, fully present.

---

## 4. Results without proof — what "proof" meant to him

This is where Ramanujan and Euler *diverge sharply* — the dossier's central contradiction, recorded
without smoothing.

**Littlewood, on the missing category — VERBATIM (quoted by Hardy, *Twelve Lectures*, via IITK excerpt):**
> "the clear-cut idea of what is meant by a proof, nowadays so familiar as to be taken for granted, he
> perhaps did not possess at all."

**Hardy on his stopping rule — VERBATIM (*Twelve Lectures*, via IITK excerpt):**
> "if a significant piece of reasoning occurred somewhere, and the total mixture of evidence and
> intuition gave him certainty, he looked no further."

Kanigel echoes it — **VERBATIM (*The Man Who Knew Infinity*, p. 359, via Wikiquote):** "once he had become
satisfied of a theorem's truth, he had scant interest in proving it to others."

**Hardy's most-quoted line about the letter's formulas — VERBATIM (*Twelve Lectures*, via IITK excerpt):**
> "They must be true because, if they were not true, no one would have had the imagination to invent
> them."

> **Contradiction with the Euler Method (do NOT smooth over).** Euler used his pentagonal-number identity
> for a decade under the honest label *"a known truth, but not yet demonstrated,"* and that labeling is
> *why his wrong conjectures never poisoned his method*. Ramanujan had **no Ledger** — "certainty from the
> total mixture" was the terminal state, not a label pending upgrade. When the certainty was right (nearly
> all the notebook results, later verified by Berndt & co.), the missing proof was a recoverable
> inconvenience; when it was *wrong* (§7), nothing caught it. Euler's honesty-labeling is exactly the
> discipline Ramanujan lacked.

---

## 5. Where the method is most visible: "Highly Composite Numbers" (1915)

Hardy singled this paper out, and the claim holds. The visible method: **exhaustive tables +
empirically-induced arithmetic laws + elephantine hand computation.**

**PARAPHRASE (Nicolas–Robin edition; MathWorld):** the 1915 *Proc. LMS* paper runs ~62 pages / ~269
numbered equations and studies "highly composite numbers" (more divisors than any smaller integer).
Ramanujan **tabulated 102 of them up to 6,746,328,388,800** by hand — the working is the tables, laid
bare, where his elegant notebook entries hide it. This is the one place the *machinery* (compute a long
table → read off the structural law → generalize) sits on the page instead of being erased.

**Hardy's split verdict — PARAPHRASE (Erdős, "Ramanujan and I"; Hardy):** "one of the most remarkable
[memoirs] published in England for many years," yet (per Erdős) "in the backwaters of mathematics" — awe
at the empirical method, mild disdain for the unfashionable subject. The paper is the exhibit of the
compute-first engine made visible.

---

## 6. The causal engine: what actually drove the output

**Appetite as the base drive — PARAPHRASE:** like Euler, inexhaustible intrinsic delight in calculation;
the γ and Bernoulli episodes are teenage, unprompted, career-valueless — the "pleasure of work over glory"
pattern, though under-documented in his own words.

**The Namagiri / divine-thought framing — HANDLE WITH CARE (firewall in §8).** Ramanujan attributed
insight to his family goddess **Namagiri Thayar of Namakkal**. Was this a *working method* or a *post-hoc
devotional framing*? Serious sources say: the direct "goddess dictated formulas in dreams" claim has
**weak primary attestation**; the best-documented Namagiri episode is his **mother Komalatammal's** dream
sanctioning his voyage (Alladi, Kanigel) — a biographical fact, not a described work-method. Treat the
divine framing as part of his *self-understanding*, not a reconstructable step.

**Isolation from formal training — the double-edged engine.** The very thing that made him original is
the thing that broke his prime work. Hardy's own counterfactual — **VERBATIM (*Twelve Lectures*):**
> "He would probably have been a greater mathematician if he could have been caught and tamed a little in
> his youth; he would have discovered more that was new, and, no doubt, of greater importance."

Hardy credits him with "profound and invincible originality" (*Twelve Lectures*, VERBATIM) and, on his
singular gift — **VERBATIM (Hardy, wording confirmed across sources):** "It was his insight into
algebraical formulae, transformation of infinite series, and so forth, that was most amazing… I can
compare him only with Euler and Jacobi." Littlewood's teaching experience shows the engine's *resistance
to correction* — **VERBATIM (MacTutor):** attempts to teach him rigor met "an avalanche of original ideas
which made it almost impossible for Littlewood to persist." The generative engine crowded out the
verifying one.

**Hardy's private rank-ordering — PARAPHRASE (Berndt, via Wikipedia):** on pure talent Hardy gave himself
**25**, Littlewood **30**, Hilbert **80**, **Ramanujan 100** — the most powerful raw engine he ever met,
which (§7) needed a governor it never had.

---

## 7. The boundary lesson: induction without theory (the prime-number failure)

The most valuable finding for the plugin: a *clean, causal* account of an S-tier method failing for want
of a specific discipline — one the Euler Method explicitly installs.

**What happened — VERBATIM (Hardy, "The Indian Mathematician Ramanujan," *AMM* 1937, p. 150):**
> "Ramanujan's theory of primes was vitiated by his ignorance of the theory of functions of a complex
> variable. It was (so to say) what the theory might be if the Zeta-function had no complex zeros. His
> method depended upon a wholesale use of divergent series… That his proofs should have been invalid was
> only to be expected. But the mistakes went deeper than that, and many of the actual results were false."

**Hardy's generalization — VERBATIM (*Twelve Lectures*, via IITK excerpt):**
> "[imagination] is a very unreliable guide… In particular this is so in the analytic theory of numbers,
> where even Ramanujan's imagination led him very seriously astray."

**The mechanism — PARAPHRASE (Hardy; Berndt, "Ramanujan's Theory of Prime Numbers"):** From particular
numerical cases Ramanujan induced a formula for π(x) and *believed it more accurate than it was*. His
induction had no access to the **complex zeros of the Riemann zeta function** — the correction terms that
oscillate and dominate the error — and implicitly assumed them absent. The pattern fit every case he
could compute by hand and **kept fitting past his fitting window**, because the zeros' effect is subtle at
accessible ranges. No amount of *more computation of the same kind* reveals the error; only the *theory he
lacked* — complex analysis — locates where the counterexample must live.

> **This is the exact failure the Euler Method's "structure theorem before the counterexample hunt" and
> "test far past the fitting window" rules exist to prevent.** Euler proving every prime divisor of F₅ has
> form 64n+1 *before* hunting, then finding 641 on the sixth division, is precisely the move Ramanujan
> could not make in analytic number theory — he didn't know the structure theorem (the zeta zeros) that
> says where the induced law breaks. **Induction that cannot be told where to look for its own
> counterexample is a loaded gun.** The same engine that produced thousands of true, deep formulas
> produced *false* theorems the instant it worked in a domain whose governing theory it lacked — and its
> internal certainty could not tell the two cases apart.

---

## 8. Folklore flags (the firewall)

- **"An equation has no meaning for me unless it expresses a thought of God."** — **FOLKLORE-FLAGGED /
  weak primary attestation.** Universally quoted as Ramanujan's mathematical creed. The traceable source
  is **S.R. Ranganathan, *Ramanujan: The Man and the Mathematician* (1967), p. 88**, given as a
  "statement to a friend" — i.e. a *devotional biography written 47 years posthumously*, not a
  contemporary record. Usable only as "reported by Ranganathan." Do not present as first-hand.

- **Namagiri dictating formulas in dreams.** — **LEGEND-UNVERIFIED as a work-method.** Hardy, per Alladi,
  **"dismissed the story of Namagiri giving the formulas to Ramanujan as a fable."** The *well-attested*
  Namagiri episode is his **mother's** permission-dream (Alladi, Kanigel), not a formula-generating dream
  Ramanujan described. **Conflict recorded:** Hardy held he was effectively agnostic and his religiosity
  romanticized ("all religions seemed equally true to him"); **Kanigel disputes Hardy**, arguing Ramanujan
  hid a rich inner spiritual life from "a man once described as 'an atheist evangelist.'" Both on the
  record; neither settled. Respect the belief as real to Ramanujan; do not launder it into a technique.

- **The taxicab 1729 story.** — **VERBATIM primary source exists; the drama is embellished.** Hardy's own
  words (*Twelve Lectures*; also 1937 essay): "I had ridden in taxi-cab No. 1729, and remarked that the
  number seemed to be rather a dull one… 'No,' he replied, 'it is a very interesting number; it is the
  smallest number expressible as the sum of two cubes in two different ways.'" (1729 = 1³+12³ = 9³+10³.)
  **Two firewall notes:** (1) C.P. Snow's *Apology* foreword dramatizes it (Hardy "inept," no greeting,
  "burst into the room" in later tellings) — Snow's flourishes, not Hardy's. (2) **Ono & Trebat-Leder
  showed Ramanujan had already recorded a³+b³=c³+d³ solutions** — second notebook, 1913–15 puzzle columns,
  lost notebook — so the "instantaneous flash" reading is almost certainly wrong: he recognized a friend,
  didn't compute on the spot (**PARAPHRASE**). The story is true and the lesson (intimacy with the numbers)
  sound; the miracle framing is folklore.

- **"Every positive integer was one of his personal friends."** — **VERBATIM, attribution itself hedged.**
  Source: **Hardy's 1921 LMS obituary, p. lvii**, phrased "It was Littlewood (I believe) who said…". Per
  search (not page-verified), Hardy first drafted "As someone said…" and only later fixed the credit — so
  even the *attribution* is a genuine "I believe." Quote it, keep the hedge.

- **The "1 + 2 + 3 + … = −1/12" claim in the first letter.** — **VERBATIM, real, and self-aware.**
  Ramanujan to Hardy (16 Jan 1913): "= −1/12 under my theory," followed by "If I tell you this you will at
  once point out to me the lunatic asylum as my goal." Not a naïve blunder — his divergent-series
  (Ramanujan-summation / ζ-regularization) technique, later made rigorous — but the same "wholesale use of
  divergent series" that *succeeded* here and *failed* in the prime theory (§7): same tool, opposite
  outcome, no internal discriminator.

---

## 9. Euler-Method map: genuine connections and hard contradictions

**Connections (real, not forced):** *Compute-first in appetite* — γ to 15 places, Bernoulli numbers
self-discovered, the e^(π√58) catch (§3). *Induction from particular numerical cases* (Littlewood) *is*
the Euler observation→conjecture arc. *Understanding over storage / the reconstruction test* — Carr's
proof-free *Synopsis*, re-derived entry by entry (§2). And Hardy himself makes the link: the one
mathematician he compares Ramanujan to for formula-insight is "Euler and Jacobi" (§6).

**Contradictions (kept sharp, as boundary lessons):**
- **Erased slate vs. published path.** Euler published his route *with false starts*; Ramanujan erased it
  and kept only the result — costing posterity the derivations Euler's method preserved for free.
- **Results without proof vs. the honest Ledger.** Euler labeled unproved truths "true but not yet
  demonstrated" and *acted on the label*; Ramanujan had certainty with no label and no upgrade-slot, so
  nothing flagged the prime results as "Observed, not Demonstrated." **That missing label is the whole
  difference between his successes staying harmless and his one big failure going uncaught.**
- **Multi-route verification.** Euler paid for every analogy with an independent check; Ramanujan "looked
  no further" once certain — his method had no second route, so in the prime case nothing contradicted the
  first.
- **Fresh-case testing past the fitting window.** Ramanujan *did* test far, but the prime counterexample
  lives at complex zeros he couldn't compute toward — testing further *in the same direction* never
  reaches it. Euler's rule needs the *structure theorem* to aim the test; that theorem (complex analysis)
  is exactly what he lacked.

---

## 10. Transferable moves (with receipts)

1. **Compute first, in appetite, and dwell on the table.** Calculate concrete cases before any theory and
   let a numerical anomaly *be* the discovery — the γ-to-15-places and e^(π√58) catches. *Receipt:*
   MacTutor; Wolfram ("experimental mathematician"). — Euler's compute-first move; adopt freely.

2. **The reconstruction test, done for real.** Don't store a result you can't re-derive; Ramanujan built
   his engine by re-deriving all ~5,000 of Carr's proof-free entries himself. *Receipt:* MacTutor, Wolfram,
   Hardy ("it awakened his genius"). — But externalize what he didn't (move 6).

3. **Make the audacious transformation — then decide whether the domain earns it.** Divergent-series work
   produced both the *correct* ζ-regularized −1/12 *and* the *false* prime theory; the missing step is
   "does this domain's theory license the manipulation?" *Receipt:* first letter (−1/12); Hardy 1937 p.150.
   — Keep the boldness, add Euler's payment-by-verification.

4. **Before hunting a pattern's limits, find the structure theorem that says where it breaks.** The prime
   failure fit every computable case yet was globally false, because the governing structure (zeta's
   complex zeros) was invisible to hand-computation. *Receipt:* Hardy 1937 p.150; *Twelve Lectures*. — The
   single most important transplant: **an induced law is only as safe as your ability to say where its
   counterexample must live**; computing further in the same direction is no substitute.

5. **Label certainty as a status, not a verdict.** Every result he "looked no further" on should have
   carried "Observed, not yet Demonstrated." *Receipt:* Littlewood ("no clear-cut idea of proof"); Hardy
   ("he looked no further"). — Imports the Euler Ledger as the missing discipline; the boundary lesson made
   operational.

6. **Record the path, not just the result — the erased slate is the anti-pattern.** Berndt spent decades
   reconstructing what a few lines would have preserved. *Receipt:* Bhāvanā (elbow-erasure); Berndt oral
   history ("no records at all"). — Scratch is disposable *for you*; write down the load-bearing route *for
   the record*.

7. **Know your friends' numbers, but don't sell recognition as revelation.** 1729 was recognizable because
   he'd *already worked* a³+b³=c³+d³ for years — familiarity, not a flash. *Receipt:* Hardy's taxicab
   account; Ono–Trebat-Leder. — Cultivate the intimacy; refuse the myth.

---

### Sources actually read this session (URLs)

- MacTutor, *Ramanujan* biography: https://mathshistory.st-andrews.ac.uk/Biographies/Ramanujan/
- Bhāvanā, "How much of Ramanujan's work has been lost?": https://bhavana.org.in/how-much-of-ramanujans-work-has-been-lost/
- Wolfram, "Who Was Ramanujan?": https://writings.stephenwolfram.com/2016/04/who-was-ramanujan/
- Wikiquote, *Srinivasa Ramanujan* (prints sourced page numbers): https://en.wikiquote.org/wiki/Srinivasa_Ramanujan
- Wikipedia, *Srinivasa Ramanujan*: https://en.wikipedia.org/wiki/Srinivasa_Ramanujan
- K. Alladi, "Touched by the Goddess," *Inference Review*: https://inference-review.com/article/touched-by-the-goddess
- J. Baez, "Hardy, Ramanujan and Taxi No. 1729," Azimuth: https://johncarlosbaez.wordpress.com/2022/01/30/hardy-ramanujan-and-taxi-no-1729/
- IITK book-excerpt of Hardy, *Twelve Lectures*: https://www.cse.iitk.ac.in/users/amit/books/hardy-1999-ramanujan-twelve-lectures.html

### Sources used only via search snippet (binary PDFs would not parse — flagged in text)

- Berndt et al., "Uncovering Ramanujan's Lost Notebook: An Oral History," arXiv:1208.2694
- "Ramanujan's Thoughts from God," arXiv:1707.03379
- Nicolas & Robin, ed., "Highly Composite Numbers" (Ramanujan Journal, 1997)
- Berndt, "Ramanujan's Theory of Prime Numbers" (*Ramanujan's Notebooks*, Springer)
- Hardy, "The Indian Mathematician Ramanujan," *Amer. Math. Monthly* 44(3), 1937 (p. 150 quote)

### Provenance caveats (do not upgrade)

- The "mingled argument…", "caught and tamed…", "profound and invincible originality," and Euler/Jacobi-
  comparison quotes are **wording-confirmed across sources** but their exact original Hardy page was **not
  personally opened this session** — VERBATIM on wording, source Hardy (*Twelve Lectures* / 1937 essay).
- The talent-scale numbers (25/30/80/100) reach us **via Berndt**, not a Hardy manuscript — PARAPHRASE.
  Claims from the two binary PDFs are flagged "via search snippet"; re-verify against readable text before
  quoting as VERBATIM.
