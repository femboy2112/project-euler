# Dossier I — Pólya's Reconstruction of Euler's Inductive Method

> Research dossier for Project EULER, compiled 2026-07-16 by a web-research agent from
> the sources listed below. Labels: **VERBATIM** (exact wording read from the source),
> **PARAPHRASE** (content confirmed, wording condensed), **UNVERIFIED** (could not be
> confirmed this session). This file is a receipt: the plugin's mode, skill, and wiki
> quote from it and must not upgrade any label.

**Primary full-text sources actually read for this dossier:**

- **[P1]** G. Pólya, *Mathematics and Plausible Reasoning, Vol. 1: Induction and Analogy in Mathematics* (Princeton UP, 1954) — complete page-image scan read via OCR page-by-page at https://www.hlevkin.com/hlevkin/90MathPhysBioBooks/Math/Polya/George_Polya_Induction_And_Analogy_In_Mathematics_1.pdf (printed pagination matches the 1954 edition — independently confirmed because Pólya's own 1959 paper cites "vol. 1, p. 91" for a quote that falls on p. 91 of this scan).
- **[P2]** Pólya, *Patterns of Plausible Inference* (Vol. 2, 2nd ed. 1968) scan, same site.
- **[D]** Euler, E175, English translation by Todd Doucet (2005): https://scholarlycommons.pacific.edu/cgi/viewcontent.cgi?filename=0&article=1174&context=euler-works&type=additional (same file as http://eulerarchive.maa.org/docs/translations/E175en.pdf). Read in full.
- **[B]** J. Bell, "Euler and the pentagonal number theorem," arXiv:math/0510054 — https://arxiv.org/pdf/math/0510054 (translations of Euler's letters/papers, full chronology).
- **[H]** R. Hersh, "Mathematical Intuition (Poincaré, Pólya, Dewey)," *The Mathematics Enthusiast* 8 (2011) — https://scholarworks.umt.edu/cgi/viewcontent.cgi?article=1205&context=tme (independent corroboration of Pólya's translations).
- **[P59]** Pólya, "Heuristic Reasoning in the Theory of Numbers," *Amer. Math. Monthly* 66 (1959) 375–384.
- Euler Archive records: E175 https://scholarlycommons.pacific.edu/euler-works/175/ ; E256 https://scholarlycommons.pacific.edu/euler-works/256/
- Sandifer, "How Euler Did It": "2aa+bb" (Jan 2006, on E256) http://eulerarchive.maa.org/hedi/HEDI-2006-01.pdf ; "A memorable example of false induction" (Aug 2005) http://eulerarchive.maa.org/hedi/HEDI-2005-08.pdf

OCR note: [P1]/[P2] quotes are transcribed from tesseract OCR of a genuine page scan; obvious single-character scanner artifacts were corrected and Euler's σ-formulas normalized. Wording and sentence structure are as printed.

---

## 1. E175 — the σ(n) recurrence memoir, as Pólya presents it (Vol. 1, Chapter VI, pp. 90–98)

### 1a. Pólya's framing and translation note

**VERBATIM** — [P1] p. 90, ch. VI §2:
> "Euler's memoir is given here, in English translation, in extenso, except for a few unessential alterations which should make it more accessible to a modern reader."
>
> Footnote: "The original is in French; see Euler's *Opera Omnia*, ser. 1, vol. 2, p. 241–253."

Pólya's title for the memoir: **"DISCOVERY OF A MOST EXTRAORDINARY LAW OF THE NUMBERS CONCERNING THE SUM OF THEIR DIVISORS"** (p. 91). Pólya substitutes σ(n) for Euler's ∫n (his footnote notes "Euler was the first to introduce a symbol for the sum of the divisors; he used ∫n").

### 1b. Euler on how he found the law by observation (Pólya's translation)

**VERBATIM** — memoir No. 1, [P1] p. 91:
> "Till now the mathematicians tried in vain to discover some order in the sequence of the prime numbers and we have every reason to believe that there is some mystery which the human mind shall never penetrate. To convince oneself, one has only to glance at the tables of the primes, which some people took the trouble to compute beyond a hundred thousand, and one perceives that there is no order and no rule. This is so much more surprising as the arithmetic gives us definite rules with the help of which we can continue the sequence of the primes as far as we please, without noticing, however, the least trace of order. I am myself certainly far from this goal, but I just happened to discover an extremely strange law governing the sums of the divisors of the integers which, at the first glance, appear just as irregular as the sequence of the primes, and which, in a certain sense, comprise even the latter. This law, which I shall explain in a moment, is, in my opinion, so much more remarkable as it is of such a nature that we can be assured of its truth without giving it a perfect demonstration. Nevertheless, I shall present such evidence for it as might be regarded as almost equivalent to a rigorous demonstration."

**VERBATIM** — memoir No. 4–5, [P1] pp. 92–93 (the observational despair → the law):
> "If we examine a little the sequence of these numbers, we are almost driven to despair. We cannot hope to discover the least order. The irregularity of the primes is so deeply involved in it that we must think it impossible to disentangle any law governing this sequence, unless we know the law governing the sequence of the primes itself. It could appear even that the sequence before us is still more mysterious than the sequence of the primes."
>
> "Nevertheless, I observed that this sequence is subject to a completely definite law and could even be regarded as a recurring sequence. This mathematical expression means that each term can be computed from the foregoing terms, according to an invariable rule."

Then the recurrence σ(n) = σ(n−1) + σ(n−2) − σ(n−5) − σ(n−7) + σ(n−12) + σ(n−15) − σ(n−22) − σ(n−26) + … with remarks I–IV (signs two-by-two; differences 1,3,2,5,3,7,4,9,… interleaving naturals and odds; drop negative arguments; **"If the sign σ(0) turns up in the formula, we must, as its value in itself is indeterminate, substitute for σ(0) the number n proposed."**) — [P1] p. 93.

### 1c. Induction vs. demonstration — Euler's explicit statements (Pólya's translation)

All **VERBATIM**, [P1]:

- No. 6, p. 93: "After these remarks it is not difficult to apply the formula to any given particular case, and so **anybody can satisfy himself of its truth by as many examples as he may wish to develop. And since I must admit that I am not in a position to give it a rigorous demonstration, I will justify it by a sufficiently large number of examples.**"
- No. 6, p. 94 (after the σ(1)…σ(20) table): "**I think these examples are sufficient to discourage anyone from imagining that it is by mere chance that my rule is in agreement with the truth.**"
- No. 8, p. 95: "**The examples that I have just developed will undoubtedly dispel any qualms which we might have had about the truth of my formula.**" (Corroborated independently in [H], p. 40.)
- No. 8, pp. 95–96 (discovery not by chance): "The lack of demonstration must increase the surprise still more, since it seems wholly impossible to succeed in discovering such a property without being guided by some reliable method which could take the place of a perfect proof. **I confess that I did not hit on this discovery by mere chance, but another proposition opened the path to this beautiful property—another proposition of the same nature which must be accepted as true although I am unable to prove it.** And although we consider here the nature of integers to which the Infinitesimal Calculus does not seem to apply, nevertheless I reached my conclusion by differentiations and other devices. I wish that somebody would find a shorter and more natural way, in which the consideration of the path that I followed might be of some help, perhaps."
- No. 9, p. 96 (the pentagonal-series identity as "known truth, not demonstrated"): "Yet I have no other evidence for this, except a long induction which I have carried out so far that I cannot in any way doubt the law governing the formation of these terms and their exponents. I have long searched in vain for a rigorous demonstration of the equation between the series and the above infinite product (1 − x)(1 − x²)(1 − x³)…, and I have proposed the same question to some of my friends with whose ability in these matters I am familiar, but all have agreed with me on the truth of this transformation of the product into a series, without being able to unearth any clue of a demonstration. **Thus, it will be a known truth, but not yet demonstrated** … **For each of us can convince himself of this truth by performing the multiplication as far as he may wish; and it seems impossible that the law which has been discovered to hold for 20 terms, for example, would not be observed in the terms that follow.**"
- No. 10, p. 96: "As we have thus discovered that those two infinite expressions are equal even though it has not been possible to demonstrate their equality, **all the conclusions which may be deduced from it will be of the same nature, that is, true but not demonstrated. Or, if one of these conclusions could be demonstrated, one could reciprocally obtain a clue to the demonstration of that equation**; and it was with this purpose in mind that I maneuvered those two expressions in many ways, and so I was led among other discoveries to that which I explained above; its truth, therefore, must be as certain as that of the equation between the two infinite expressions."
- No. 13, p. 98 (closing): "This reasoning, although still very far from a perfect demonstration, will certainly lift some doubts about the most extraordinary law that I explained here."

(For comparison, Doucet [D] renders the "qualms" sentence as "These examples that I have just developed will no doubt remove any scruple which one could still have about the truth of my formula" — same content, different translator.)

### 1d. The mechanics Pólya highlights: cases computed, fresh tests, cross-checks

- **Table of observations:** memoir No. 4 gives a table of σ(n) for n = 1 to 99 in Pólya's arrangement ([P1] p. 92; Doucet's translation of the original runs to ∫100 = 217). VERBATIM.
- **Explicit verification of the recurrence for n = 1,…,20** — the full worked list σ(1)…σ(20) appears at [P1] p. 94 (e.g. "σ(20) = σ(19) + σ(18) − σ(15) − σ(13) + σ(8) + σ(5) = 20 + 39 − 24 − 14 + 15 + 6 = 42"). VERBATIM.
- **Fresh cases not used to find the law** — memoir No. 7, [P1] p. 94: "Yet somebody could still doubt whether the law of the numbers 1, 2, 5, 7, 12, 15, … which we have to subtract is precisely that one which I have indicated, **since the examples given imply only the first six of these numbers. Thus, the law could still appear as insufficiently established and, therefore, I will give some examples with larger numbers.**"
  - **σ(101):** "I. Given the number 101, find the sum of its divisors. … = 893 − 791 = 102 … and hence we could conclude, if we would not have known it before, that 101 is a prime number." ([P1] p. 94)
  - **σ(301):** "II. Given the number 301, find the sum of its divisors. … Performing the computations, we find σ(301) = 4939 − 4587 = **352**. We see hence that 301 is not a prime. In fact, 301 = 7 · 43 and we obtain σ(301) = σ(7)σ(43) = 8 · 44 = 352 **as the rule has shown**." ([P1] p. 95) — the unproven law is used to *compute* a new value, then cross-checked against the independently known factorization. VERBATIM.
- **"Over 300 cases"** (primary source behind the memoir): Euler's letter to Goldbach, April 1, 1747 (Letter 113), trans. in [B] §4: "**However, if I had no proof at all, one would still not be able to doubt the truth of it, because over 300 cases always follow this rule.**" Also: "I have recently discovered a very amazing order in the integers… since in this a great connection with the order of the prime numbers appears to hide." And on the conditional structure: "if this statement is true, which I do not doubt, despite the fact that I do not have a rigorous demonstration, then the theorem is completely justified." VERBATIM from [B].
- E175 was presented to the Berlin Academy on **June 22, 1747**, published in *Bibliothèque impartiale* 3 (1751), pp. 10–31 ([B]; Euler Archive record E175).

---

## 2. E256 "Specimen de usu observationum in mathesi pura" — the observation manifesto

**VERBATIM — Pólya's English translation, quoted as the epigraph opening Chapter I ("Induction") of Vol. 1, p. 3** (checked twice against the scan; this is the passage the whole book opens with):

> "It will seem **not a little paradoxical** to ascribe a great importance to observations even in that part of the mathematical sciences which is usually called Pure Mathematics, since the current opinion is that observations are restricted to physical objects that make impression on the senses. As we must refer the numbers to the pure intellect alone, we can hardly understand how observations and quasi-experiments can be of use in investigating the nature of the numbers. Yet, in fact, as I shall show here with very good reasons, the properties of the numbers known today have been mostly discovered by observation, and discovered long before their truth has been confirmed by rigid demonstrations. There are even many properties of the numbers with which we are well acquainted, but which we are not yet able to prove; only observations have led us to their knowledge. Hence we see that in the theory of numbers, which is still very imperfect, we can place our highest hopes in observations; they will lead us continually to new properties which we shall endeavor to prove afterwards. The kind of knowledge which is supported only by observations and is not yet proved must be carefully distinguished from the truth; it is gained by induction, as we usually say. Yet we have seen cases in which mere induction led to error. Therefore, we should take great care not to accept as true such properties of the numbers which we have discovered by observation and which are supported by induction alone. Indeed, we should use such a discovery as an opportunity to investigate more exactly the properties discovered and to prove or disprove them; in both cases we may learn something useful. —EULER"
>
> Pólya's footnote: "Euler, *Opera Omnia*, ser. 1, vol. 2, p. 459, Specimen de usu observationum in mathesi pura."

Context on E256 itself (Euler Archive record; Sandifer HEDI-2006-01): written 1754, presented Berlin 22 Nov 1753 / St. Petersburg 30 Sep 1754, published 1761 in *Novi Commentarii* 6, pp. 185–230; the body studies numbers of the form 2a²+b² — Euler tabulates all such numbers below 500, states eight observations, then spends 15 pages proving what he can. Sandifer (PARAPHRASE): Euler here "decided to 'come clean' about how he knew what to try to prove."

---

## 3. The pentagonal number theorem story

- **The hand expansion** — Euler, E175 memoir No. 9, Pólya's translation ([P1] p. 96, VERBATIM): "In considering the partitions of numbers, I examined, a long time ago, the expression (1−x)(1−x²)(1−x³)(1−x⁴)(1−x⁵)(1−x⁶)(1−x⁷)(1−x⁸)… in which the product is assumed to be infinite. **In order to see what kind of series will result, I multiplied actually a great number of factors** and found 1 − x − x² + x⁵ + x⁷ − x¹² − x¹⁵ + x²² + x²⁶ − x³⁵ − x⁴⁰ + …"
- **How far he went:** in E158 ("Observationes analyticae variae de combinationibus," presented St. Petersburg April 6, 1741) §36 he prints the series to n⁵¹ and says: "**Here at the end of this dissertation a noteworthy observation should be made, which however I have not been able to demonstrate with geometric rigor**" ([B], VERBATIM). In the letter to Goldbach of Oct 15, 1743 he continues the series to n⁵⁷ and writes "**it is easily shown by induction** that all of the terms are contained in the form n^((3xx±x)/2)… **I have however not yet found a method by which I could prove the identity of these two expressions. The Hr. Prof. Niklaus Bernoulli has also been able to prove nothing beyond induction**" ([B], VERBATIM).
- **The long wait and mounting conviction** — Euler to Goldbach, May 6, 1747 ([B], VERBATIM): "I have also only been able to conclude by induction, **which I however have continued so far, that I consider the matter completely true; I would be very enthusiastic to see a direct proof of this matter**… hitherto all of my pains have been for nothing." Goldbach (Apr 15, 1747) had answered that the induction made it credible "one-hundred to one" ([B]).
- **The proof, ~1750:** letter to Goldbach, **June 9, 1750** (Letter 144; [B], VERBATIM): "**Since that time however I have also found a demonstration of this theorem**, which depends on this lemma: (1−α)(1−β)(1−γ)(1−δ) etc. = 1 − α − β(1−α) − γ(1−α)(1−β) − … whose demonstration is immediate." Published in E244, "Demonstratio theorematis circa ordinem in summis divisorum observatum," *Novi Commentarii* 5 (1760), 75–83, where Euler writes that now "**Not any doubt may remain of this property**" ([B]). So the identity ran **~9–10 years unproven** (1740/41 → June 1750). (Note: Pólya's book itself does not date the later proof; the chronology is from [B]'s primary sources.)
- Pólya's ch. VI examples reprise the theme (ex. 6.21, [P1] p. 106, VERBATIM): "For us this latter is a conjecture. We derived this conjecture, as Euler has derived his, 'by differentiation and other devices' from another conjecture."

---

## 4. Pólya's own distilled rules of plausible reasoning drawn from Euler

- **The inductive attitude** — [P1] pp. 7–8, ch. I §4 (VERBATIM): "In our personal life we often cling to illusions… but in science we need a very different attitude, the *inductive attitude*. This attitude aims at adapting our beliefs to our experience as efficiently as possible… It requires saying 'maybe' and 'perhaps' in a thousand different shades. It requires many other things, especially the following three. First, we should be ready to revise any one of our beliefs. Second, we should change a belief when there is a compelling reason to change it. Third, we should not change a belief wantonly, without some good reason. … The first point needs 'intellectual courage.' … The second point needs 'intellectual honesty.' … The third point needs 'wise restraint.' … **Intellectual courage, intellectual honesty, and wise restraint are the moral qualities of the scientist.**"
- **The fundamental inductive principle** — [P1] p. 7 (VERBATIM): "We seem to accept a principle: **A conjectural general statement becomes more credible if it is verified in a new particular case.**"
- **Verification of consequences (from the Euler ζ(2) case study)** — [P1] pp. 21–22, ch. II §6 (VERBATIM): "(1) **Euler's decisive step was daring. In strict logic, it was an outright fallacy**… Yet it was justified by analogy, by the analogy of the most successful achievements of a rising science that he called himself a few years later the 'Analysis of the Infinite.'… (2) Euler's reasons for trusting his discovery… are not demonstrative. **Euler does not reexamine the grounds for his conjecture… he examines only its consequences. He regards the verification of any such consequence as an argument in favor of his conjecture.** He accepts both approximative and exact verifications… He examines also the consequences of closely related analogous conjectures… **Euler's reasons are, in fact, inductive.** … He seems to accept certain principles: **A conjecture becomes more credible by the verification of any new consequence. And: A conjecture becomes more credible if an analogous conjecture becomes more credible.**"
- **The schematic outline of Euler's memoir** — [P1] pp. 99–100, ch. VI §§3–4 (VERBATIM key lines): "we are concerned here not so much with the mathematical content of this theorem, but rather with **the reasons which induced Euler to believe in the theorem when it was still unproved**." The outline abstracts the memoir into theorems T (product = pentagonal series) and T* (the σ-recurrence): "Theorem T includes an infinite number of particular cases… I have made these calculations and I find that C₁, C₂, C₃, …, C₄₀ are all true… **Theorems T and T\* are equivalent; they are both true or false; they stand or fall together.** … By examination, I find that **C\*₁₀₁ and C\*₃₀₁ are true, and so I find that theorem T\* is valid even for these cases which are far removed from those which I examined earlier.**"
- **Strength of inductive evidence (three criteria)** — [P1] pp. 68–70, ch. IV §8 (VERBATIM key lines): "**Number of verifications**… **Precision of prediction**… it is obviously reasonable to assume… that **the verification of a more precise prediction carries more weight than that of a less precise prediction**… **Rival conjectures**… Other things being equal, a conjecture that has many obvious rivals is more difficult to accept than one that is unrivalled." Plus the flat refusal to numerify: "What is the precise, objectively evaluated degree of rational belief…? … To solve this problem is much more than I can do."
- **Nature of inductive discovery ("hoping for a law")** — [P1] p. 68, ch. IV §7 (VERBATIM): "What have we obtained? Not a proof, not even the shadow of a proof, just a conjecture: a simple description of the facts within the limits of our experimental material, **and a certain hope that this description may apply beyond the limits of our experimental material.** How have we obtained our conjecture? … We collected relevant observations, examined and compared them, noticed fragmentary regularities, hesitated, blundered, and eventually succeeded in combining the scattered details into an apparently meaningful whole."
- **Analogy and the "hope for a common ground"** — Vol. 2 [P2], ch. XIII §9 (2nd ed., p. 27; VERBATIM): "let us consider the analogy of two theorems A and B as **the intention to discover a common ground H** from which both A and B would follow… **Let us not forget that we do not have H; we just hope that there is such an H.**"
- **Chapter V epigraph** — [P1] p. 76 (VERBATIM): "**When you have satisfied yourself that the theorem is true, you start proving it.** —THE TRADITIONAL MATHEMATICS PROFESSOR"

---

## 5. Pólya on Euler's uniqueness

**VERBATIM** — [P1] p. 90, ch. VI §1 "Euler," with Condorcet epigraph:
> Epigraph: "He [Euler] preferred instructing his pupils to the little satisfaction of amazing them. He would have thought not to have done enough for science if he should have failed to add to the discoveries, with which he enriched science, the candid exposition of the ideas that led him to those discoveries. —CONDORCET"
>
> "Of all mathematicians with whose work I am somewhat acquainted, Euler seems to be by far the most important for our inquiry. **A master of inductive research in mathematics, he made important discoveries (on infinite series, in the Theory of Numbers, and in other branches of mathematics) by induction, that is, by observation, daring guess, and shrewd verification.** In this respect, however, Euler is not unique; other mathematicians, great and small, used induction extensively in their work. **Yet Euler seems to me almost unique in one respect: he takes pains to present the relevant inductive evidence carefully, in detail, in good order. He presents it convincingly but honestly, as a genuine scientist should do.** His presentation is 'the candid exposition of the ideas that led him to those discoveries' and has a distinctive charm. Naturally enough, as any other author, he tries to impress his readers, but, as a really good author, he tries to impress his readers only by such things as have genuinely impressed himself."

**VERBATIM** — Pólya interview at 90 (G. L. Alexanderson, *Two-Year College Mathematics Journal* 10 (1979) 13–19), read at https://divisbyzero.com/2010/03/01/polya-on-euler/ (secondary but directly quoted):
> "…among old mathematicians, I was most influenced by Euler and mostly because Euler did something that no other great mathematician of his stature did. He explained how he found his results and I was deeply interested in that. It has to do with my interest in problem solving."

---

## Flags / could-not-verify / discrepancies caught

1. **"It will seem *not* a little paradoxical" vs. "a little paradoxical":** Wikiquote (and sources copying it) drop the "not." The 1954 book scan reads "**not a little paradoxical**" (verified against [P1] p. 3). Use the "not" version when quoting Pólya.
2. **"…not fortified by rigorous demonstration":** NOT found in Pólya's book or any accessible E256 translation. Treat as a variant/misremembered translation — unverified.
3. **Doucet translation typo:** [D] prints "∫301 = 353" twice (verified visually). The arithmetic and Pólya's book both give **352**. Cite 352.
4. **Extent of Euler's σ-table:** Pólya's arrangement shows σ(1)–σ(99) (condensed per his footnote); Doucet's translation of the original lists through ∫100 = 217. Not a contradiction.
5. **No full English translation of E256 exists** in the Euler Archive/arXiv that was accessible; only Pólya's excerpt (the introduction) plus Sandifer's summary of the body. Pólya's book does not date the pentagonal theorem's proof — the 1750 chronology rests on Bell's translations of the Goldbach correspondence and E244.
6. **"Mere induction led to error" — Euler's own examples:** Euler later published a worked cautionary tale, "Exemplum memorabile inductionis fallacis" (in E326, *Observationes analyticae*, 1765/1767): two natural rules for the central trinomial coefficients agree for nine terms (through 3139) then diverge (8953 vs 8955) — documented in Sandifer HEDI-2005-08.
7. **Access caveat:** the hlevkin scans are third-party-hosted copies of the Princeton editions. Quotes above are fair-use-scale excerpts transcribed for scholarship; page numbers refer to the printed 1954 edition (Vol. 1) and 1968 2nd edition (Vol. 2).
