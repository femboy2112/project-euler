# Dossier III — The Technical Anatomy of Euler's Method

> Research dossier for Project EULER, compiled 2026-07-16 by a web-research agent.
> Labels: **VERBATIM** / **PARAPHRASE** / **UNVERIFIED**, with flags for commonly
> misstated items. This file is a receipt: the plugin quotes from it and must not
> upgrade any label.

**Verification basis:** 15 "How Euler Did It" columns (Ed Sandifer, MAA Online, 2003–2010) downloaded from `eulerarchive.maa.org/hedi/` and read as text; E-number records from the Euler Archive (`eulerarchive.maa.org/backup/Exxx.html`); Jordan Bell's English translation of E41 (arXiv), Ian Bruce's translation of E45, Varadarajan's and Lagarias's Bulletin AMS surveys, and others listed per episode.

---

## 1. The Basel Problem (E41, 1735): compute first, prove second, cross-check third

### (a) The numerical reconnaissance (1730–1735)

- **E20**, *De summatione innumerabilium progressionum* (Commentarii 5 (1730/31), pub. 1738): Euler transforms ζ(2) into the rapidly convergent form ζ(2) = (log 2)² + 2·Σ 1/(n²·2ⁿ). Sandifer: "Euler uses a very clever approximation technique to get a numerical value, **1.644924**, for this integral. The series itself converges rather slowly, and you would have to sum more than 30,000 terms to get this degree of accuracy directly." **[VERBATIM**, HEDI-2003-12]. Lagarias confirms **[VERBATIM]** and adds: direct summation to six decimals "would require taking into account at least a million terms." *Flag:* Varadarajan prints "1.644944" — almost certainly a typo; Sandifer and Lagarias agree on 1.644924.
- Sandifer on the payoff: "among his other skills, Euler is a fantastic calculator. He sees this value is close to π²/6. Armed with this hint, he begins to attack the Basel Problem using series for trigonometric functions." **[VERBATIM**, HEDI-2003-12].
- **The ~20-decimal computation is E47, not E25.** **E25** (presented June 20, 1732) states the Euler–Maclaurin formula without proof; **E47** (written ~1734/35) gives details, introduces Bernoulli polynomials, "and also applied his summation formula to obtain **ζ(2) and ζ(3) to 20 decimal places**" **[VERBATIM**, Lagarias §2.4]. Sandifer (HEDI-2007-10): Euler found Euler–Maclaurin "at least eight years before Maclaurin's work."
- In **E41 itself** (§2, Bell translation): "Indeed I recently showed for the sum of this series to be approximately **1,644934066842264364**; multiplying this number by six, and then taking the square root, the very same number **3,141592653589793238** is found" **[VERBATIM]**. *Flag:* the printed ζ(2) string has a typographical slip (drops an "8"; true value 1.6449340668**48**2264365...); the π value is correct to all 18 printed places. The match was Euler's private certificate of correctness before any proof existed.

### (b) The audacious move (E41, presented December 5, 1735)

- E41, *De summis serierum reciprocarum*: "read in the St. Petersburg Academy on December 5, 1735" **[PARAPHRASE**, Euler Archive]; published Commentarii 7 (1734/35), 1740.
- Mechanism (Bell translation, §§4–9): Euler treats the equation sin s = y written as an infinite-degree polynomial: "if in this equation s is seen as an unknown, it will have infinitely many degrees, and it will not be surprising that this equation should contain countless simple factors" **[VERBATIM]**. He applies the Newton relations wholesale (recursion P = α; Q = Pα − 2β; R = Qα − Pβ + 3γ; ... **[VERBATIM**, §8]) — generating *all* even power sums at once.
- With y = 0 (§16–17), the sine product: "1 − s²/(1·2·3) + s⁴/(1·2·3·4·5) − ... = (1 − s²/p²)(1 − s²/4p²)(1 − s²/9p²)... etc." **[VERBATIM**; note E41 uses **p** for π]. From this: ζ(2) = p²/6; ζ(4) = p⁴/90; up to **ζ(12), where 691 surfaces** (the Bernoulli fingerprint) **[VERBATIM** table, §18].

### (c) The cross-checks

- Recovering Leibniz (§10): 1 − 1/3 + 1/5 − 1/7 + ... = p/4, and Euler writes: "And indeed this is the very same series discovered some time ago by Leibniz, by which he defined the quadrature of the circle. **From this, if our method should appear to some as not reliable enough, a great confirmation comes to light here; thus there should not be any doubt about the rest that will be derived from this method.**" **[VERBATIM**, Bell trans. §10]. This is the explicit epistemology: a new method must reproduce known results before its novel outputs are trusted.
- Further checks in E41: the Newton (y = 1/√2) series = p/(2√2) (§14); alternating cubes = p³/32 (§12); ζ(4) = p⁴/90 obtained **twice** (biquadrates route and product route) **[PARAPHRASE]**; the prior 18-digit numerical value as standing confirmation.

### (d) Criticism and the later proofs

- "Euler communicated his original proof to his correspondents... **Daniel Bernoulli criticized it on the grounds that sin πx may have other complex roots**" **[VERBATIM**, Lagarias p. 542, citing Ayoub and Weil]. Varadarajan states the two standard objections: missing roots, and eˢf(s) having the same roots as f(s) **[VERBATIM]**. *Flag:* Sandifer (HEDI-2004-03) calls the eˢ objection "a modern objection, not raised in Euler's time" — in tension with the Weil/Ayoub record on the complex-roots worry; both reported.
- Euler's responses: (i) "Nevertheless the numerical evaluations bolstered Euler's confidence, and he kept working... It took him about ten years, but he finally succeeded in obtaining the famous product formula for sin s... Once this formula is established, all the objections disappear, as he himself remarked" **[VERBATIM**, Varadarajan pp. 519–520]; rigorous route in **E61** (1743) and the Introductio (1748). (ii) A **completely independent proof**: **E63** (1741, pub. 1743, in French, "a seldom-read paper... in a rather obscure literary journal"): from s = arcsin x, integrate arcsin(x)·dx/√(1−xx) via the binomial series, getting π²/8 = 1 + 1/9 + 1/25 + ...; Sandifer: "all it requires to meet modern standards of rigor is that we fill in a few routine steps and notice that a few series are absolutely convergent" **[VERBATIM**, HEDI-2004-03].
- **How many proofs?** Lagarias: "In December 1735, in [E41]... Euler gave **three** proofs that ζ(2) = π²/6" **[VERBATIM/PARAPHRASE]**. With E63, E61/Introductio, and E212's Bernoulli-number route: "three in E41 itself, at least three more methodologically distinct routes by 1755" is the defensible count.

---

## 2. Divergent Series: E247 and the functional equation (E352)

### E247, De seriebus divergentibus

- Dates: "written in 1746, but not read to the Academy until 1754, nor published until 1760" **[VERBATIM**, Sandifer HEDI-2006-06]. (Varadarajan: "communicated in 1755" — minor discrepancy.)
- **The definition, verbatim** (Barbeau–Leah translation, quoted in Varadarajan pp. 526–527): "Understanding of this question is to be sought in the word 'sum'; this idea, if thus conceived — namely the sum of a series is said to be that quantity to which it is brought closer as more terms of the series are taken — has relevance only for convergent series, and we should in general give up this idea of sum for divergent series. ... if we employ this definition of sum, that is to say, **the sum of a series is that quantity which generates the series**, all doubts with respect to divergent series vanish and no further controversy remains on this score." **[VERBATIM]**. And: "always a closed formula from whose expansion the series arises should be investigated" **[VERBATIM]**.
- Pre-history: 1745 letters to Goldbach and N. Bernoulli on Σ(−1)ⁿn! ("the divergent series par excellence"): "I believe that every series should be assigned a certain value. However... this value should not be denoted by the name sum, because usually this word is connected with the notion that a sum has been obtained by a real summation" **[VERBATIM**, Varadarajan's translation, p. 527].
- **The consistency-check discipline** — for A = 1 − 1! + 2! − 3! + ...: (1) Euler's difference-transformation formula iterated three times; (2) divergent series for 1/A and log A ("similar methods also lead to a value of A near 0.59"); (3) continued fractions for A and 1/A; (4) the ODE method: s = x − 1x² + 2x³ − 6x⁴ + ... satisfies ds/dx = (x−s)/x², solved to A = e·∫₀¹ (e^(−1/x)/x)dx, evaluated by 10-point quadrature as **0.59637255**; "By the end of the article, Euler has estimated A at least **six very different ways**, and every time he gets the same estimate." **[VERBATIM/PARAPHRASE**, Sandifer HEDI-2006-06]. Via the continued fraction (E247's own summary): "the author by a wholly singular method using continued fractions found that the sum of this series is about **0.596347362123**, and in this decimal fraction the error does not affect even the last digit" **[VERBATIM**, Barbeau–Leah trans.]. Modern check: 0.5963473623231940... — all 12 digits correct. Borel summation avant la lettre.
- Varadarajan's caveat: "He appeared to believe that all series could be summed by some procedure or other and also that in general all summation procedures would lead to the same value. The actual theory of divergent series shows that the situation is much more subtle." **[VERBATIM**, p. 527].

### E352 — the zeta functional equation, a century before Riemann

- **E352**, *Remarques sur un beau rapport entre les séries des puissances tant directes que réciproques*: presented Berlin 1749; published 1768 **[PARAPHRASE**, Euler Archive + cross-checks].
- Euler worked with η(s) = (1−2^(1−s))ζ(s) "for better convergence and more accurate numerical evaluation" and conjectured the functional equation η(1−s)/η(s) = −(2ˢ−1)/((2^(s−1)−1)πˢ) · cos(sπ/2) · Γ(s) **[PARAPHRASE**, Varadarajan pp. 528–529]. He deliberately wrote (−1)^k as cos kπ — "clearly suggesting that he was thinking of the functional equation for non-integral values of s. Euler then proceeded to write that '... I shall hazard the conjecture that the relation... is true for all s...'" **[VERBATIM**, Varadarajan's rendering of "je hasarderai la conjecture"].
- **How he verified it:** exactly for every integer s (positive, negative, zero — using even-zeta values, η(0) = 1/2, η(1) = log 2, and Γ(s)Γ(1−s) = π/sin sπ); exactly at s = 1/2; and **numerically for half-integers**: "For s = 3/2 Euler used the Euler–Maclaurin sum formula to compute the sums appearing on both sides... it appears that he had verified the functional equation for s = (2i+1)/2 (i = 1, 2, ...)... Euler went ahead because he firmly believed that all methods of summation lead to the same value. ... Much later Landau justified Euler's method of summation for all s." **[VERBATIM**, Varadarajan p. 529]. Riemann proved it 110 years later.

---

## 3. Refutation: factoring F₅ = 2³² + 1 (E26, E134, E283)

- **Trigger:** P.S. of Goldbach's first letter (December 1, 1729), Latin quoted by Sandifer: "Notane Tibi est Fermatiana observatio omnes numeros hujus formulae 2^(2^x) + 1, nempe 3, 5, 17, etc. esse primos, quam tamen ipse fatebatur se demonstrare non posse et post eum nemo, quod sciam, demonstravit." **[VERBATIM**, HEDI-2003-11]. Euler "responded almost immediately that he could make no progress" but had the refutation by 1732 **[PARAPHRASE**, HEDI-2007-03].
- **E26** (presented September 26, 1732): announces 641 | 4,294,967,297 — "though he does not give any clues about how he discovered this fact" **[VERBATIM**, Euler Archive summary] — plus six unproven "theorems," the first being Fermat's Little Theorem **[PARAPHRASE]**.
- **The smart part, revealed in E134** (read March 23, 1747): from his now-proved FLT machinery, culminating in **Theorem 8: "The sum of two such powers a^(2^m) + b^(2^m), in which the exponents are powers of two, will not admit any divisors except those that are contained in the form 2^(m+1)·n + 1."** **[VERBATIM**, Sandifer's translation, HEDI-2007-03]. Applied to F₅ with m = 5: every prime divisor has form **64n + 1**. Sandifer walks the search: 193 (fails), 257 (fails), 449 (fails), 577 (fails), **n = 10 → 641 divides, quotient 6,700,417**. "We find the factor 641 after just six divisions." **[VERBATIM]**. The anatomy of Eulerian refutation: prove a structure theorem to collapse the search space, then search.
- The cofactor: "Euler did not speculate in print on whether the other factor, 6,700,417, is prime. It is prime, but there is no evidence that Euler ever tried to find out." **[VERBATIM/PARAPHRASE**, HEDI-2007-03].
- **E283** (presented December 1, 1760): "reproves that F5 is not prime. Euler provides factor tables for aa + 1, for a < 1500" **[VERBATIM**, Euler Archive]. ***Flag (commonly misstated):*** the sharpened divisor form k·2^(n+2) + 1 is **Lucas (1878)**, not Euler.
- **Other Euler (self-)refutations:**
  - **E326** (written 1763), section titled **"EXEMPLUM MEMORABILE INDUCTIONIS FALLACIS"**: central trinomial coefficients 1, 1, 3, 7, 19, 51, 141, 393, 1107, 3139, ... versus a Fibonacci-built rule that reproduces the first **nine** terms and then breaks: "this has 8955 where there should be an 8953, and after that the differences become even larger... There really are two different sequences, each defined by reasonable and interesting patterns that agree for the first nine terms, and then become different." **[VERBATIM**, Sandifer HEDI-2005-08]. Sandifer pairs it with E256: "Ten years later, he gives us a graphic illustration of the limits of observation, and that it shows mathematicians what might be true, not necessarily what is true." **[VERBATIM]**.
  - **A wrong Euler conjecture in the multizeta letters** (January 19, 1743): his claimed ζ*(6,2) evaluation "is false, and so were a few others. In fact, this one isn't even very close" **[VERBATIM/PARAPHRASE**, Sandifer HEDI-2008-01].
  - **Scientific self-corrections** (HEDI-2008-02 "Fallible Euler"): lunar atmosphere (E142), aether friction (E89, E183/184, E218), bubble model of air (E7, E527). Even when wrong: observation → quantitative model → proposed discriminating test **[PARAPHRASE]**.

---

## 4. Königsberg (E53, 1735/36): what Euler actually did

- **Chronology (verified):** presented St. Petersburg **August 26, 1735** (Euler Archive; arXiv:1505.02411); published as *Solutio problematis ad geometriam situs pertinentis*, Commentarii 8 (1736), printed **1741**; 21 numbered paragraphs.
- **The letters (attributions verified — commonly swapped):**
  - **Ehler to Euler, March 9, 1736:** "You would render to me and our friend Kühn a most valuable service, putting us greatly in your debt, most learned Sir, if you would send us the solution, which you know well, to the problem of the seven Königsberg bridges, together with a proof. It would prove to be an outstanding example of Calculi Situs, worthy of your great genius." **[VERBATIM**, arXiv:1505.02411].
  - **Euler to Ehler, April 3, 1736:** "... Thus you see, most noble Sir, how this type of solution **bears little relationship to mathematics**, and I do not understand why you expect a mathematician to produce it, rather than anyone else, for the solution is based on reason alone, and its discovery does not depend on any mathematical principle..." **[VERBATIM**, arXiv:1505.02411].
  - **Euler to Marinoni, March 13, 1736:** "A problem was posed to me about an island in the city of Königsberg... **This question is so banal, but seemed to me worthy of attention** in that geometry, nor algebra, nor even the art of counting was sufficient to solve it. In view of this, it occurred to me to wonder whether it belonged to the geometry of position, which Leibniz had once so much longed for. And so, after some deliberation, I obtained a simple, yet completely established, rule..." **[VERBATIM** as reproduced at mathsweek.ie, deriving from Sachs–Stiebitz–Wilson/Hopkins–Wilson].
- **E53's opening:** "Besides that part of geometry which is concerned with quantities... there is another part, still quite unknown, of which Leibnitz was the first to make mention and which he called *geometria situs*, the geometry of position." **[VERBATIM**, Behrend translation, §1].
- **The actual argument (vs. the modern retelling):** Euler never draws a graph. He encodes walks as **letter sequences**: regions A–D; a walk over seven bridges is a string of eight letters; if n bridges touch region A and n is odd, A must occur (n+1)/2 times; summing required occurrences (A:5→3, B,C,D:3→2 each; 3+2+2+2 = 9 > 8 slots) gives the impossibility. General rule (§20): "If there are more than two regions with an odd number of bridges leading into them, then it can safely be stated that there is no such crossing..." **[VERBATIM**, Behrend trans.].
- **What he did *not* prove:** sufficiency. §21 waves at it: "...then let a walk be planned across the remaining bridges, **which is easily done**" **[VERBATIM]**. Sufficiency was first rigorously proved by **Carl Hierholzer (1873)** **[PARAPHRASE]**. The dots-and-lines diagram appears nowhere in E53; the graph rendering is a 19th-century addition (commonly attributed to Rouse Ball 1892 — reported secondhand, not verified).

---

## 5. Notation: what Euler introduced or standardized (verified list)

| Symbol | First use / standardization | Source |
|---|---|---|
| **f(x)** | **E45**, *Additamentum ad dissertationem de infinitis curvis eiusdem generis*, presented **July 12, 1734**, pub. 1740: "if f(x/a + c) denotes some function of x/a + c ..." — first functional notation with parenthesized argument. *Flag:* often cited as "E44"; the notation is in the Additamentum, E45. | Euler Archive E045; 17centurymaths.com E45 trans.; MacTutor Miller |
| **e** | First written in unpublished E853 (1727/28): "For the number whose logarithm is unity, let e be written, which is 2,7182817..." **[VERBATIM via MacTutor]**; first letter: to Goldbach, Nov 25, 1731; first print: Mechanica, 1736. | MacTutor Miller "constants" |
| **π** | William Jones 1706 (first use for 3.14159...). Euler used **p** for π in E41 itself; adopted π in Mechanica (1736); the Introductio (1748) made it universal. | MacTutor; E41 trans.; HEDI-2009-02 |
| **i for √−1** | Memoir presented **May 5, 1777** (E671), pub. posthumously 1794: "formulam √−1 littera i in posterum designabo, ita ut sit ii = −1" **[VERBATIM via MacTutor]**. Standardized by Gauss (1801). | MacTutor; HEDI-2007-08 |
| **Σ for summation** | **E212** (1755): "Quemadmodum ad differentiam denotandam vsi sumus signo Δ, ita summam indicabimus signo Σ." **[VERBATIM via MacTutor]** | MacTutor "operation" |
| **sin, cos as functions** | Introductio, **1748**, ch. 8: "the first time that anyone treats sines, cosines, etc. as **functions** rather than as ratios" **[VERBATIM**, Sandifer HEDI-2007-08]. Euler never wrote e^(iπ)+1=0 itself — Sandifer documents this at length. | HEDI-2007-08 |
| **γ (constant, not symbol)** | Discovered in **E43** (1734; ≈0.577218, 6 printed/5 correct digits); 15–16 places in E212 (1755). The **symbol γ was probably not Euler's or Mascheroni's** — earliest verified: Bretschneider (1835/37). "I think it was probably Bretschneider." **[VERBATIM**, HEDI-2007-10] | HEDI-2007-10 |

---

## 6. Euler–Maclaurin and computation as instrument

- **The tool:** E25 (1732, statement) → E47 (details, Bernoulli polynomials) → E212 Part II ch. 5–6 (1755; Bernoulli numbers through n = 15, with Euler's remark that they "form a highly divergent sequence, which grows more strongly than any geometric series" **[VERBATIM via Lagarias]**). It took him "20 years to discover" the Bernoulli-number identity of his coefficients (Sandifer HEDI-2007-10).
- **γ:** E43 (1734): ≈0.577218 (5 correct). E212 (1755): γ to **15–16 places** via Euler–Maclaurin with divergent-tail truncation (Lagarias reproduces: C = 0.5772156649015325). E583: tests whether e^γ = 1.78106... is a "notable number": "One may suspect from this that the number C is the hyperbolic logarithm of some notable number... it will be worthwhile to inquire into the value of this number N" **[VERBATIM via Lagarias]** — computing *in order to conjecture*; he fails to match it and says so. ***Flag:*** "γ to 16 digits in E43" conflates E43 (6 digits) with E212/E583.
- **ζ values:** E47: ζ(2), ζ(3) to 20 places. Letter to Goldbach, Feb 26, 1743: "eighteen-place decimal approximations to ζ(n) through n = 16" **[VERBATIM**, Sandifer HEDI-2008-01].
- **π:** **E74** (1737): survey of π computation, arctangent identities. **E705** (1779): transformed arctangent series engineered for decimal-friendly ratios: "Euler seeks the best of both worlds, rapid convergence and easy calculations." "Euler calculates the first of these series accurately to 12 decimal places and the second to 17 places, but for some reason he doesn't add them together to give an approximation of π." **[VERBATIM**, HEDI-2009-02]. ***Flag (commonly misstated):*** "Euler computed 20 digits of π in one hour" has **no support in the primary record as read by Sandifer** — treat as folklore.
- **Tables:** the Introductio teaches generation: logs of 2, 5, 10 to seven places, the Briggs trick, fast-converging trig series **[PARAPHRASE**, HEDI-2005-07]. Continued fractions as rigor instrument: **E71** (1737) contains the expansion of (e−1)/2 giving the first proof that **e is irrational** **[PARAPHRASE**, HEDI-2006-02].
- The general point, Varadarajan: "no one who calculated the values of many convergent series to tremendous accuracy would have loose ideas about when series diverge and what their values are" **[VERBATIM**, p. 527].

---

## 7. Serial return: the same problems across decades (documented chains)

- **Zeta/Basel chain:** E20 (1730/31) → E25 (1732) → E43 (1734) → E47 (~1734/35) → **E41 (Dec 5, 1735)** → E72 (1737: the **Euler product**) → E130 (1739) → E61 + Goldbach letters (1741/42) → E63 (1743) → multizeta letters (1742–43) → Introductio (1748) → **E352 (1749: functional equation)** → E212 (1755) → E393 (1768) → **E477 (1771, pub. 1776: returns to multizeta after ~30 years**, grinding cases to n = 9 over "more than 12 pages" until "the pattern is evident" [Sandifer HEDI-2008-01]). Span: **1730 → 1776**.
- **Partitions:** Naudé's letter, Sept 4, 1740 → E158 (read April 6, 1741; "this may be where generating functions are first used"; answer to Naudé: 522) → Introductio ch. 16 (1748) → E191 (1750) → pentagonal theorem proved in **E244** (pub. 1760) → **E394 (1769)** "Late in his life... he returned to the problem" [HEDI-2005-10]. Span: **1740 → 1769**.
- **Fermat little/last theorems:** Goldbach P.S. (Dec 1, 1729) → E26 (1732) → **E54** (1736: first published proof of FLT; "When he first discovered the theorem in 1732, he apparently did not know of Fermat's work on the subject" **[VERBATIM**, HEDI-2003-11]) → **E134** (1747: second proof + divisor theorems) → **E271** (1758: third proof, the totient generalization) — "over the course of forty years, Euler published at least three different proofs" **[VERBATIM]**. FLT cases: n=4 (E98), n=3 (Algebra, 1770). Span: **1729 → 1770s**.
- **Elliptic integrals:** E252 (presented Jan 27, 1752) — addition theorems developed after reading Fagnano (the "birthday of elliptic functions" framing is standard lore, not primary-verified). **[PARAPHRASE]**.
- Production by decade (Sandifer HEDI-2005-08): 1720s: 11, 1730s: 67, 1740s: 114, 1750s: 131, 1760s: 111, **1770s: 309**, 1780s: 67 — the blind decade is the most productive; papers "continued to appear until 1862, 79 years after his death" **[VERBATIM]**.

---

## Sources actually read (URLs)

**Sandifer, "How Euler Did It"** (all at `http://eulerarchive.maa.org/hedi/HEDI-YYYY-MM.pdf`): 2003-11 (Fermat's Little Theorem), 2003-12 (Estimating the Basel Problem), 2004-03 (Basel Problem with Integrals), 2005-07 (Finding logarithms by hand), 2005-08 (False induction), 2005-09 (Bernoulli numbers), 2005-10 (Philip Naudé's problem), 2006-02 (Who proved e is irrational?), 2006-06 (Divergent series), 2007-03 (Factoring F5), 2007-08 (e, π and i), 2007-10 (Gamma the constant), 2008-01 (Multi-zeta functions), 2008-02 (Fallible Euler), 2009-02 (Estimating π).

**Other:** Euler E41 trans. Bell — https://arxiv.org/pdf/math/0506415 • E45 trans. Bruce — http://www.17centurymaths.com/contents/euler/e045tr.pdf • Varadarajan, "Euler and his work on infinite series," Bull. AMS 44 (2007) — https://www.ams.org/journals/bull/2007-44-04/S0273-0979-07-01175-5/S0273-0979-07-01175-5.pdf • Lagarias, "Euler's constant," Bull. AMS 50 (2013) — https://www.ams.org/journals/bull/2013-50-04/S0273-0979-2013-01423-X/S0273-0979-2013-01423-X.pdf • Euler Archive records E019–E352 at `http://eulerarchive.maa.org/backup/Exxx.html` • arXiv:1505.02411 (Ehler/Marinoni letters) • E53 trans. Behrend — https://www.cantab.net/users/michael.behrend/repubs/maze_maths/pages/euler_en.html • Wikipedia "Seven Bridges of Königsberg" • MacTutor/Jeff Miller "Earliest Uses" pages • mathsweek.ie Königsberg page.

## Consolidated flags (could not verify / commonly misstated)

1. **"π to 20 digits in an hour"** — folklore; contradicted by E705's primary record.
2. **"ζ(2) to ~20 places via E25"** — method is E25's; the computation is **E47** (ζ(2) *and* ζ(3)); E41's printed value has a dropped-digit typo.
3. **E20's printed estimate**: 1.644924 (Sandifer, Lagarias) vs Varadarajan's 1.644944 (typo).
4. **k·2^(n+2)+1** — Lucas (1878), not Euler; Euler proved k·2^(n+1)+1 (E134).
5. **f(x) is E45, not E44.**
6. **Königsberg letter quotes frequently swap-attributed**: "so banal... worthy of attention" = Marinoni letter; "bears little relationship to mathematics" = Ehler letter. Hopkins & Wilson (2004) and Sachs–Stiebitz–Wilson (1988) were not directly accessible; quotes cross-confirmed via arXiv:1505.02411 + two secondaries. "First graph drawing = Rouse Ball 1892" reported secondhand.
7. **E247 reading date**: 1754 (Sandifer) vs 1755 (Varadarajan). **E352 presentation**: 1749 (most sources) vs 1761 (one modern source).
8. **"γ to 16 digits in E43"** — E43 gives 6 printed/5 correct; 15–16 digits are E212 (1755).
9. **"Euler gave N proofs of Basel"** — three in E41 itself (Lagarias); ~six distinct routes by 1755; no canonical lifetime total.
10. Sandifer's "modern objection" aside vs the Weil/Ayoub record of D. Bernoulli's complex-roots criticism — both reported.
