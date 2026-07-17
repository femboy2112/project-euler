# Dossier VI — Gauss and Newton: the Working Method (and its Anti-Patterns)

> Research dossier for Project EULER's "masters' wing," compiled 2026-07-16 by a web-research agent.
> Labels: **VERBATIM** (exact wording read from source), **PARAPHRASE** (content confirmed,
> wording condensed), **LEGEND-UNVERIFIED** (circulates but no primary attestation traceable).
> This file is a receipt: the plugin quotes from it and must not upgrade any label.
>
> **Mission note.** A study of METHOD, not biography and not a results catalog: what each man DID at
> the desk, the causal engine, which moves transplant to a modern session — and where the method
> carried documented ANTI-PATTERNS. Both men have publication pathologies Euler did not; those
> contrasts are as valuable as the positive moves.

**Scope note on sources.** Where a primary manuscript exists and is digitized, it was read directly:
De Moivre's memorandum and Stukeley's memoir via the Newton Project (Oxford); Newton's "prime of my
age" memorandum via the Add MS 3968 dispute papers. For the two firewall cases — the Gauss schoolroom
sum and the "I have had my results for a long time" quote — the provenance literature (Hayes 2006;
Wikiquote's sourcing thread) was read to establish what the earliest source actually says.

---

## 1. GAUSS — Compute-first at Eulerian scale: the prime-counting program

**The 1849 letter to Encke (24 December 1849) — VERBATIM (standard English translation):**
> "Your remarks concerning the frequency of primes were of interest to me in more ways than one.
> You have reminded me of my own endeavors in this field which began in the very distant past, in
> 1792 or 1793, after I had acquired the Lambert supplements to the logarithmic tables. ... I soon
> recognized that behind all of its fluctuations, this frequency is on the average inversely
> proportional to the logarithm, so that the number of primes below a given bound n is approximately
> equal to ∫ dn/log n, where the logarithm is understood to be hyperbolic."

Gauss was 72 when he wrote this; the work described was done at **age ~15–16**. A widely reproduced
rendering of the same letter has him say counting primes "in several chiliads" (blocks of a thousand)
was "one of my first projects" — **PARAPHRASE** (translation varies; the "chiliad" language is
faithful to the German *Chiliade* and to his surviving tally sheets). His *Nachlass* contains the
counts of primes in every chiliad up to a million. **This is the single strongest Euler parallel in
the dossier:** empirical compute-first at appetite scale, the density law *observed* from tables
~1792–93, and the theory (the logarithmic integral) trusted and refined privately for **~57 years
before he told anyone in print** — he never published the prime-count law at all; Legendre published
a fitted form (1798/1808) first. (nonagon.org Ex Libris; Goldstein, "A History of the Prime Number
Theorem"; arXiv:1311.1093.)

**Engine:** the density law was not deduced — it was *seen in the table* and then believed. Same move
as Euler dwelling on a table before conjecturing. The difference is entirely downstream: Euler would
have printed the table and the guess; Gauss filed both.

---

## 2. GAUSS — The mathematical diary (Tagebuch): the working rhythm made visible

**PARAPHRASE (cross-confirmed Wikipedia "Gauss's diary"; hellenicaworld; Springer critical survey):**
A small book of ~19 pages, **146 dated entries, kept 1796–1814**. Lost for decades; **discovered by
Paul Stäckel in 1897** in the *Nachlass* of a Gauss grandson at Hameln; **published by Felix Klein in
1903** (reprinted Werke X.1). It is the private lab-notebook of the most productive stretch of his life.

**First entry — VERBATIM (Latin, 30 March 1796):**
> "Principia quibus innititur sectio circuli, ac divisibilitas eiusdem geometrica in septemdecim
> partes etc." — the ruler-and-compass construction of the regular **17-gon** (heptadecagon), the
> first advance on constructible polygons in ~2000 years, discovered when he was 18.

**Entry 18 — VERBATIM (Greek/Latin, 10 July 1796):**
> "ΕΥΡΗΚΑ! num = Δ + Δ + Δ" — his proof that every positive integer is a sum of three triangular
> numbers (a case of Fermat's polygonal-number theorem). Having learned Greek, he spelled *Eureka* as
> Archimedes would have. (tandfonline, "The Eureka theorem of Gauss," *Math. Gazette* 108/571, 2024;
> ProofWiki.)

**Method reading — and the anti-pattern in the same object.** The diary shows the genuine Eulerian
rhythm: a *dated* stream of observations, one discovery logged the instant it landed, the same topics
returned to over eighteen years. **But it is results-only.** The entries record *what* he found, almost
never *how* — no derivations, no failed paths, often deliberately cryptic. Where Euler's memoirs
"exposed the path he chose to follow, the difficulties and the detours" (Dossier II §6), Gauss's
notebook is the opposite instrument: a proof-of-priority ledger written for no reader. The habit that
made the diary — record the ripe result, hide the road to it — is the seed of §4's anti-pattern.

---

## 3. GAUSS — "Pauca sed matura" (few, but ripe)

**The motto — VERBATIM (Latin):** "Pauca sed matura" — *few, but ripe*.
**Attestation — PARAPHRASE:** reported as the motto of his personal **seal**, whose device is a **tree
bearing a few fruits** (the "ripeness" pun made literal). Attested in Sartorius von Waltershausen's
memorial (1856) and in Bell, *Men of Mathematics* (1937) — the Wikiquote sourcing thread confirms
"Bell DOES say ... 'Pauca sed matura' was Gauss's motto." The heraldry is independently documented
(Numericana, "Coat-of-arms of Carl Friedrich Gauss"). *Label note:* the Latin motto and the tree-seal
are solidly attested; the exact number of fruits varies between retellings, so treat "seven fruits" as
unverified ornament. **Verdict: PARAPHRASE, well-attested.**

**What it meant in practice — VERBATIM (his own gloss, via the standard biographies):** he would not
release a result "until it was complete and he was entirely satisfied with its presentation." He
compared a finished proof to a building from which the scaffolding has been removed — the reader should
not see the construction. This is the *explicit doctrinal inverse* of the Euler Method's
publish-the-path / show-the-failed-attempts discipline, and Gauss defended it as a virtue.

---

## 4. GAUSS — The documented COST of secrecy (the sharpest anti-pattern)

**Non-Euclidean geometry, buried alive.** Gauss had the essentials of hyperbolic geometry decades
before Bolyai and Lobachevsky and published none of it.

- **To Bessel, 27 January 1829 — VERBATIM (standard translation):** "it may be that I shall never put
  [these researches] into a form fit for publication in my lifetime, since I fear the **clamor of the
  Boeotians** were I to speak out in full." ("Boeotians" = proverbial dullards.)
- **To Schumacher — PARAPHRASE (MacTutor):** he "believed his reputation would suffer if he admitted in
  public that he believed in the existence of such a geometry."
- **On János Bolyai's 1832 *Appendix* — VERBATIM (letter to Farkas Bolyai, the father):** "To praise it
  would amount to praising myself. For the entire content of the work ... coincides almost exactly with
  my own meditations which have occupied my mind for the past thirty or thirty-five years." **The
  documented human cost — PARAPHRASE (encyclopedia.com; MacTutor):** the letter "robbed [János] of the
  priority ... had such a discouraging influence on him that he withdrew into himself more and more, and
  for long periods he did hardly any mathematics." Pauca sed matura did not just cost *Gauss* credit; it
  broke a rival genius who had gotten there independently.

**The pattern repeats.** Elliptic functions: the diary shows Gauss anticipated results later published
by Abel and Jacobi — unpublished. Least squares: Gauss claimed private use from 1795 but **Legendre
published first (1805)**, producing a bitter priority dispute that Gauss's silence had armed. In every
case the engine is the same and so is the failure mode: ripe fruit left on the private tree until
someone else grew their own.

**Contrast with Euler (explicit):** Euler donated priority freely (Maclaurin, Daniel Bernoulli,
Lagrange — Dossier II §4) and printed even his dead ends. Gauss hoarded ripe results and let the
priority wars come. Same intrinsic drive; opposite public ethic. **This is the plugin's central
contradiction and belongs in the folklore firewall as a *method* warning, not a quote.**

---

## 5. GAUSS — Ceres, 1801: directed computation under a deadline (de-embellished)

**PARAPHRASE (cross-confirmed math.berkeley.edu presentation; MacTutor; arXiv:2108.06305):** Piazzi
discovered Ceres on 1 January 1801 and tracked it for ~40 days over ~24 observations before it was lost
in the Sun's glare. The 24-year-old Gauss computed an orbit from the sparse arc; **Zach relocated Ceres
on 7 December 1801** (Olbers on 1 January 1802) close to Gauss's prediction. The visible method is
massive *directed* hand-computation from minimal data under time pressure — Eulerian in appetite and in
stakes.

**Firewall caveat — flag honestly:** the popular "Gauss used least squares to find Ceres" is *partly
retrospective*. He "did not disclose his methods at the time" (MacTutor); he published the machinery
only in *Theoria Motus* (1809). Historians note "some ambiguity as to whether Gauss actually applied
the theory of least squares in computing the [1801] orbit." **Label: the deadline-computation is
documented (PARAPHRASE); the specific least-squares-for-Ceres mechanism is DISPUTED — do not state it as
fact.**

---

## 6. NEWTON — The anni mirabiles, in his own words

**VERBATIM (Newton's own memorandum, written c.1716–18, among the Add MS 3968 fluxions-dispute papers;
reproduced in Westfall, *Never at Rest*, and the Cambridge *Isaac Newton* vol.):**
> "... All this was in the two years of 1665 and 1666, for in those years I was in the prime of my age
> for invention, and minded Mathematics and Philosophy more than at any time since."

The surrounding passage lists the fluxions method, the theory of colours, the inverse method of
fluxions, and gravity "extending to the orb of the Moon" — all in the plague years at Woolsthorpe. *Label
note:* this is Newton's own late-life reconstruction, written **fifty years after the fact and during
the Leibniz priority war**, so it is self-interested testimony about dates; but as a statement of his
*working self-image* — total absorption in one appetite-driven stretch — it is first-person VERBATIM.

**Method reading:** the anni mirabiles are the archetype of the *dwell* run at maximum — a young mind
"minding Mathematics and Philosophy more than at any time since," undistracted, for two years.

---

## 7. NEWTON — How he made discoveries: the dwell, stated as method

**VERBATIM (reported reply, in *Biographia Britannica*, 1760, vol. 5, p. 3241 — the earliest traceable
source):**
> "I keep the subject constantly before me, and wait 'till the first dawnings open slowly, by little and
> little, into a full and clear light."

The compressed form "By always thinking unto them" (his reported answer to *how* he made discoveries)
circulates from the same tradition. **Label: PARAPHRASE / reported saying.** The wording is VERBATIM *as
printed in Biographia Britannica*, but that is 1760 — 33 years after Newton's death — and no contemporary
eyewitness is named; it is a reported saying, not a documented conversation. Do **not** cite it as a
letter or a firsthand quote.

**Method reading:** this is the purest available statement of the Euler-style *dwell* — sustained,
patient attention held on one object until structure emerges. "Wait till the first dawnings open little
by little" is the same discipline as Euler dwelling on a table before conjecturing, or "chance favors the
prepared mind."

---

## 8. NEWTON — The computation appetite (and a labeling correction)

**The hyperbola to 52 figures — VERBATIM (Newton's own memorandum, via D.T. Whiteside, *Mathematical
Papers*):** during the plague, summer 1665, Newton "computed the area of the Hyperbola at Boothby, in
Lincolnshire, **to two and fifty figures** by the same method" (the method of infinite series he had
found the previous winter). The manuscript survives. Computing a logarithm-area to **52 decimal places**
by hand, for no external purpose, is compute-first appetite at Eulerian scale. (flashman.neocities.org;
encyclopedia.com, "Sir Isaac Newton.")

**The "ashamed to tell" remark — VERBATIM, but MISLABELED in the mission brief — flag this:**
> "I am ashamed to tell you to how many figures I carried these computations, having no other business at
> the time."

This remark is Newton on his **π computation** (an arcsine series, 1666, carried to ~15 published
digits), **not** on the hyperbola area. Both are genuine, both are the same appetite, and the two are
routinely conflated. **Label: the 52-figures hyperbola computation and the "ashamed to tell" π remark are
two separate documented facts about the same plague-year appetite — keep them distinct.** (This is a
firewall labeling win: the seductive single sentence — "he computed the hyperbola to 52 places and was
ashamed to tell how far he'd carried it" — welds two true facts into one false one.)

---

## 9. NEWTON — Self-teaching by serial return (De Moivre's memorandum)

**VERBATIM (Abraham de Moivre's memorandum on Newton, 1727; Newton Project OTHE00034):** on how the young
Newton taught himself from Descartes' *Géométrie* —
> "read some few pages in it, then stop't; began again, went a little farther than the first time, stopt
> again, went back again to the beginning, read on till by degrees he made himself master of the whole."

**On Euclid — VERBATIM (same memorandum):** he "read only the titles of the propositions, which he found
so easy to understand that he wondred how any body would amuse themselves to write any demonstrations of
them." **On Oughtred — VERBATIM:** he read Oughtred but "understood [it] tho not entirely," stuck on the
"*Scala secundi et tertii gradus*" (solving quadratics and cubics).

**Method reading — a direct hit on two Euler-doctrine moves.** (a) *Serial return:* restart from the top,
each pass going further than the last — the same "never abandons a topic, returns relentlessly" habit Weil
identified in Euler. (b) *Understanding-over-storage / reconstruction:* Newton did not memorize Descartes,
he **rebuilt** the whole from repeated passes until he owned it — the reconstruction test, run on himself,
in 1664.

---

## 10. NEWTON — Method-signature: "ex ungue leonem"

**VERBATIM (Johann Bernoulli, letter to Basnage, March 1697):** on receiving Newton's *anonymous* solution
to the brachistochrone challenge, Bernoulli recognized the author "as the lion by its claw" — *ex ungue
leonem*. **Label note:** the often-quoted expanded form "*tanquam ex ungue leonem*" is David Brewster's
1855 phrasing (PARAPHRASE), not Bernoulli's. **The all-nighter — PARAPHRASE (Conduitt memorandum,
secondhand):** Newton found the problem in his post after returning from the Mint at 4 p.m. on 29 January
1697, worked until ~4 a.m., and sent the anonymous solution next day. (Brachistochrone: Wikipedia;
Sussmann, Rutgers.)

**Method reading (on-topic):** the point is not the speed; it is that a rigorous method leaves a
*recognizable signature* — the work of a disciplined mind is identifiable by its structure even unsigned.
That is a property worth engineering into one's own method.

---

## 11. NEWTON — The apple (attested testimony, precisely labeled)

**VERBATIM (William Stukeley, *Memoirs of Sir Isaac Newton's Life*; recording a conversation of **15 April
1726**; MS completed 1752, digitized and published by the Royal Society 2010; Newton Project OTHE00001):**
> "... why should that apple always descend perpendicularly to the ground, thought he to himself;
> **occasion'd by the fall of an apple**, as he sat in a contemplative mood."

**Label: attested testimony, NOT pure legend — but Newton's own late-life recollection.** This is Newton,
at ~83, telling Stukeley over dinner in the garden about an event ~60 years earlier. It is the *earliest
and best* source for the apple and it is a real primary document — so it is not folklore — but it is a
reminiscence, not a contemporary record, and the "apple hit his head" embellishment appears in *neither*
Stukeley nor Newton. Cite as: Newton's own recollection, via Stukeley, of the apple as the *occasion* (not
the cause) of the gravitation thought.

---

## 12. NEWTON — The publication anti-pattern → the Leibniz war

**PARAPHRASE (cross-confirmed Wikipedia "Leibniz–Newton controversy"; maths.tcd.ie Commercium account):**
Newton developed fluxions in **1665–66**; wrote *De Analysi* in **1669** (circulated to Barrow and Collins)
but did **not publish it until 1711**; the *Principia* (1687) used deliberately geometric methods that hid
the calculus; the first published account of his method was "a minor annotation in the back of one of his
publications decades later" (*De Quadratura*, appended to the *Opticks*, 1704). Leibniz published the
differential calculus in **1684**. The suppression is what made the priority question *possible*: by the
time Newton's method was public, Leibniz's was established and independently developed.

**The pathology compounds:** when the war came (~1699–1712), Newton, as President of the Royal Society,
arranged the "impartial" investigating committee, and **wrote its verdict himself** — the *Commercium
Epistolicum* (1712), published anonymously and finding for Newton. **~30–45 years of hoarding produced the
ugliest priority dispute in the history of mathematics.**

**Contrast with Euler:** Euler published continuously, in appetite, and gave credit away. Newton hoarded
for decades and then weaponized an institution to defend the hoard. Together with Gauss's *pauca sed
matura*, this is the masters' wing's dominant negative lesson.

---

## 13. Folklore flags (things NOT to repeat as fact)

- **The Gauss schoolroom sum (1 + 2 + ⋯ + 100) — LEGEND-UNVERIFIED in its modern form. FIREWALL ENTRY.**
  Brian Hayes, "Gauss's Day of Reckoning" (*American Scientist* 94, 2006, p. 200), cataloged ~**70 tellings**
  and traced them to the earliest source, **Sartorius von Waltershausen, *Gauss zum Gedächtnis* (1856)**.
  **VERBATIM finding (Hayes):** what is most remarkable about the Sartorius telling "is not what's there but
  what's absent. There is no mention of the numbers from 1 to 100, or any other specific arithmetic
  progression. And there is no hint of the trick or technique that Gauss invented to solve the problem."
  The specific series (1–100), the slates, the pupils racing, and Gauss's dialect exclamation "**Ligget
  se'**" ("there it lies") are **later accretions**. The kernel — a small boy stuns schoolmaster Büttner —
  is Sartorius-attested but sparse. Do not state the 1-to-100 version, the pairing trick, or "Ligget se'" as
  documented fact. (bit-player.org, "A Mathematical Fable Revisited," is Hayes's follow-up.)

- **"I have had my results for a long time: but I do not yet know how I am to arrive at them" (Gauss) —
  LEGEND-UNVERIFIED / attributed.** Universally quoted; the nearest cited source is **Sartorius (1856),
  p. 79**, but Wikiquote flags it "**[Attributed]**" and no clean primary was traced this session. The
  common secondary attribution route runs through **Arago**, which could **not** be confirmed. Usable only
  as "attributed; nearest source Sartorius 1856, unverified." *Irony worth noting:* if genuine, it is the
  purest statement of the results-before-path habit that §2–§4 identify as Gauss's signature and his flaw.

- **The apple hitting Newton's head — LEGEND.** Absent from Stukeley (§11) and from Newton's own account;
  the apple *fell* and *occasioned a thought* — it did not strike him.

- **"Tanquam ex ungue leonem"** — the *tanquam* is Brewster's 1855 embellishment; Bernoulli wrote *ex
  ungue leonem* (§10).

- **"Newton computed the hyperbola to 52 places and was ashamed to tell how far he carried it"** — a WELD
  of two true facts into one false one; the 52-figures was the hyperbola area, the "ashamed to tell" remark
  was the π computation (§8). Keep them separate.

- **"Gauss used least squares to relocate Ceres"** — DISPUTED; he concealed his 1801 method and published
  least squares only in 1809 (§5).

---

## 14. Transferable moves (with receipts) — and the named anti-patterns

**Positive moves (these transplant to a modern working session):**

1. **Compute-first at appetite scale, before any theory.** Gauss counted primes through chiliads to a
   million by hand and *saw* the 1/ln n density law in the tally (Encke letter, §1); Newton computed a
   hyperbola-area to 52 decimal places for no external purpose (§8). Receipt: the density law was observed
   ~1792–93, decades before any proof existed. **Move:** generate the big table first; let the law announce
   itself.

2. **The dwell, stated as method: "keep the subject constantly before you and wait till the first dawnings
   open little by little."** (Newton, §7.) Sustained, patient, single-object attention is the engine, not a
   flash. **Move:** hold one problem in view across many sessions rather than demanding an answer now.

3. **Serial return / reconstruct-until-you-own-it.** Newton read Descartes by restarting from the top,
   each pass going further, "till by degrees he made himself master of the whole" (De Moivre memorandum,
   §9). This is the reconstruction test run on a text: don't store it, rebuild it until you can regenerate
   it. **Move:** re-derive load-bearing results from scratch instead of memorizing; if you can't rebuild it,
   you don't own it.

4. **Keep a dated discovery log — the Tagebuch habit (§2) — BUT publish the path.** The log itself is a
   genuinely great instrument (146 dated entries across 18 years, one discovery captured the instant it
   lands). The *failure* was making it results-only and private. **Move:** keep the dated ledger; then, unlike
   Gauss, write up the derivation and the dead ends. (This is exactly Project EULER's Ledger doctrine.)

5. **Engineer a recognizable method-signature.** Newton's anonymous work was identifiable "by the lion's
   claw" (§10) because his *method* had a structural signature. **Move:** aim for work whose rigor is
   recognizable independent of the byline.

**The named anti-patterns (as valuable as the moves above):**

- **THE SECRECY ANTI-PATTERN — "pauca sed matura" / the 30-year hoard.** Gauss withheld non-Euclidean
  geometry ("clamor of the Boeotians," §4), crushing János Bolyai's independent priority and discouraging
  him out of mathematics; anticipated elliptic functions and least squares into priority disputes; and made
  his notebook a private proof-of-priority ledger. Newton hoarded the calculus ~30–45 years, then wrote the
  Royal Society's "impartial" verdict for himself (§12). **The lesson, stated as method:** withholding *ripe*
  results does not protect them — it poisons priority, crushes rivals who arrive independently, and starves
  the field. Euler's publish-the-path (credit donated freely, failed attempts printed) is the antidote and
  the reason his wrong conjectures never poisoned his method.

- **THE HIDDEN-PATH NOTEBOOK.** Recording *what* you found without *how* (Gauss's diary, §2; the seal's
  "scaffolding removed" doctrine, §3) defeats reconstruction and understanding-over-storage. A log that
  hides its derivations is a priority claim, not a method.

**One-line engine statements.**
- **Gauss:** *observe the pattern in a vast hand-built table, trust the ripe result privately, and publish
  nothing until it is a building with the scaffolding removed* — Eulerian observation married to an
  anti-Eulerian silence.
- **Newton:** *keep one subject constantly before the mind through years of undistracted dwell until the
  first dawnings open into full light — then tell almost no one for thirty years.*

---

## 15. Sources actually consulted (URLs)

**Gauss.** Encke letter (nonagon.org): https://nonagon.org/ExLibris/origin-prime-number-theorem-legendre-gauss • Goldstein PNT history: https://jontalle.web.engr.illinois.edu/uploads/298.16/GoldsteinHistPrimeNumThm.73.pdf • log-integral origin: https://arxiv.org/pdf/1311.1093 • Diary: https://en.wikipedia.org/wiki/Gauss's_diary and https://www.hellenicaworld.com/Science/Mathematics/en/GausssDiary.html • Eureka theorem: https://www.tandfonline.com/doi/abs/10.1017/mag.2024.15 • Heraldry/motto: https://www.numericana.com/arms/gauss.htm • Wikiquote sourcing thread: https://en.wikiquote.org/wiki/Talk:Carl_Friedrich_Gauss • Non-Euclidean/Bolyai/Boeotians: https://mathshistory.st-andrews.ac.uk/Biographies/Gauss/ and https://www.encyclopedia.com/science/dictionaries-thesauruses-pictures-and-press-releases/bolyai-janos-johann • Ceres: https://math.berkeley.edu/~mgu/MA221/Ceres_Presentation.pdf and https://arxiv.org/pdf/2108.06305 • Schoolroom firewall (Hayes): https://www.americanscientist.org/article/gausss-day-of-reckoning and http://bit-player.org/2007/a-mathematical-fable-revisited/ • Sartorius 1856: https://archive.org/details/gauss00waltgoog

**Newton.** De Moivre memorandum (primary): https://www.newtonproject.ox.ac.uk/view/texts/normalized/OTHE00034 • Stukeley memoir/apple (primary): https://newtonproject.ox.ac.uk/view/texts/normalized/OTHE00001 • Royal Society apple MS: https://royalsociety.org/blog/2012/02/newtons-apple-tree/ • "Prime of my age" memorandum: https://www.cambridge.org/core/books/abs/isaac-newton/prime-of-my-age-for-invention-16641667/6998078731EC0B670EB51249CB6857D5 • Newton Institute life: https://www.newton.ac.uk/about/isaac-newton/isaac-newtons-life/ • "First dawnings" (Biographia Britannica 1760): https://en.wikiquote.org/wiki/Isaac_Newton • Hyperbola to 52 figures: https://flashman.neocities.org/Presentations/Estimations and https://www.encyclopedia.com/people/science-and-technology/physics-biographies/sir-isaac-newton • Brachistochrone/ex ungue leonem: https://en.wikipedia.org/wiki/Brachistochrone_curve and https://sites.math.rutgers.edu/~sussmann/papers/brachistochrone-mex.pdf • Calculus priority/Commercium: https://en.wikipedia.org/wiki/Leibniz%E2%80%93Newton_calculus_controversy and https://www.maths.tcd.ie/pub/HistMath/People/Newton/CommerciumAccount/
