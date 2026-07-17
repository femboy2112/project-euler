# Dossier VIII — The Moderns: Working Methods of Erdős, Grothendieck, Feynman, Tao

> Research dossier for Project EULER (masters' wing), compiled 2026-07-16 by a web-research agent.
> Labels: **VERBATIM** (exact wording read from source), **PARAPHRASE** (content confirmed,
> wording condensed), **LEGEND-UNVERIFIED** (circulates without a traceable primary attestation).
> This file is a receipt: the plugin quotes from it and must not upgrade any label.
> Scope: METHOD ONLY — what each figure actually DID, the causal engine, the transplantable moves.
> Not biography, not a results catalog. Failures, limits, and anti-patterns are findings.

**Scope note on sources.** Primary documents read in full or near-full this session: Colin McLarty's
essay *The Rising Sea* (the R&S translations quoted are McLarty's own, stated in his fn.1); W. T.
Gowers, *The Two Cultures of Mathematics* (PDF, downloaded and read); László Babai, *In and Out of
Hungary* (PDF, read — note pdftotext dropped c/f ligatures, reconstructed against the published Straus
quote); Terence Tao's four career-advice blog pages (primary source, living Fields medalist); Pierre
Cartier's Grothendieck memoir in *Inference*; the Aigner–Ziegler *Proofs from THE BOOK* preface (via
Quanta + Wikipedia); Quote Investigator on the coffee aphorism; the Rogers Commission transcript
(vol. 4) for the O-ring; Rota's *Ten Lessons* (Notices AMS, via fs.blog verbatim capture, the AMS PDF
was 403). URLs at the foot of the file.

---

## 1. PAUL ERDŐS — the problem-poser as institution

**What he actually did.** Erdős did not run a research program; he ran a *problem economy*. The
central act was posing sharply-stated hard problems and routing them to whoever could solve them.

**No program, only problems — VERBATIM (Babai, quoting E. G. Straus, "Paul Erdős at 70," ref [36]):**
> "In this century, in which mathematics is so strongly dominated by 'theory constructors,' he has
> remained the prince of problem solvers and the absolute monarch of problem posers. ... [A] great
> mathematician ... complained to me that 'Erdős only gives us corollaries of the great metatheorems
> which remain unformulated in the back of his mind.'"

Straus adds the line the plugin will care about — **VERBATIM (Straus, via Babai):** "In many ways,
Paul Erdős is the Euler of our times." (The comparison is Straus's, made explicitly on the grounds
that Erdős's "special" problems, like Euler's, seeded whole disciplines — combinatorial and
probabilistic number theory, combinatorial geometry.) Babai's own framing — **PARAPHRASE:** Erdős
"has never declared a program of research nor stated a general mathematical objective," and was "the
universal thesis advisor: it is believed that at least a hundred mathematicians have reached tenured
positions by working on problems he has proposed."

**The prize economy — how he priced difficulty.** Prizes were a difficulty *gauge*, not a wage.
**VERBATIM (Ronald Graham, via Quanta 2017):** "Here's a nice problem, I thought about it for a
while, and I don't see how to solve it. Maybe it's a $25 problem or possibly a $100 problem." Range
ran "**$25 into the thousands**, depending on how challenging he thought the problem was" (Quanta,
PARAPHRASE). Documented payouts: **$1,000** to Szemerédi (1974); a **$10,000** problem on prime gaps
(collected 2014 by Ford, Green, Konyagin, Maynard, Tao) that Graham said Erdős regarded even at the
time as "a bit **rash**" (Quanta, VERBATIM fragment). The economy outlived him: Graham administers the
fund and still pays claims. *Engine:* the price is a **public, calibrated conjecture about
inaccessibility** — it broadcasts "this is exactly how far past the tools I think this sits," which is
itself information.

**Collaboration at scale — the traveling salesman.** Erdős had **~511 coauthors** (Erdős number 1;
counts of 509–512 circulate by date — see folklore flag). Itinerant, homeless by choice, he arrived on
doorsteps announcing **"My brain is open"** (John Tierney, *Discover* / NYT, the phrase Babai cites at
ref [38]; also the title of Schechter's biography). Babai (PARAPHRASE): Erdős was "a catalyst of
interaction between mathematicians, making introductions wherever he sensed shared mathematical
interests." *Engine:* he was a **human router** — he held thousands of open problems and hundreds of
solvers in his head and made the matches, a distributed research network with Erdős as the switchboard.

**"The Book" — elegance as compass.** Erdős invoked a book in which God (the "SF," Supreme Fascist,
his joking name) keeps the perfect proof of every theorem. **VERBATIM (Erdős, 1985 lecture, reported
in Aigner–Ziegler, *Proofs from THE BOOK*, preface):** "You don't have to believe in God, but you
should believe in The Book." His highest praise for a proof: *"This one is from The Book."* → Direct
tie to the **Euler doctrine of re-derive-for-elegance**: elegance is not decoration, it is the signal
that you have found the *right* proof, the one worth remembering.

**Anti-pattern / limit (documented, on-mission).** Gowers's *Two Cultures* essay is the serious source
ON the problem-solver vs. theory-builder distinction, and it names Erdős as the archetype of one pole.
**VERBATIM (Gowers), the two priorities:** "(i) The point of solving problems is to understand
mathematics better. (ii) The point of understanding mathematics is to become better able to solve
problems." **VERBATIM (Gowers) on Erdős:** "Paul Erdős, who bequeathed to the world an enormous number
of fascinating problems, as well as solutions to many others, but is not associated to the same extent
with the development of theory." Gowers also records the field's bias — **VERBATIM:** "the subjects
that appeal to theory-builders are, at the moment, much more fashionable than the ones that appeal to
problem-solvers." The honest limit: Erdős's method deliberately *declined* to build the theory his own
corollaries pointed at ("the great metatheorems which remain unformulated in the back of his mind").
A method that maximizes problems solved can under-invest in the framework that would make whole
classes of them trivial — which is precisely Grothendieck's countermove below.

---

## 2. ALEXANDER GROTHENDIECK — the rising sea

**What he actually did.** He refused to attack a hard theorem head-on. He *dissolved* it: generalize
the setting until the theorem becomes an obvious consequence of the right definitions, then the
original problem is barely worth stating.

**The two styles — VERBATIM (Grothendieck, *Récoltes et Semailles*, pp. 552–3, trans. McLarty).**
The hammer-and-chisel: "put the cutting edge of the chisel against the shell and strike hard. If
needed, begin again at many different points until the shell cracks — and you are satisfied." The
rising sea, in his own words:
> "I can illustrate the second approach with the same image of a nut to be opened. The first analogy
> that came to my mind is of immersing the nut in some softening liquid, and why not simply water?
> From time to time you rub so the liquid penetrates better, and otherwise you let time pass. The
> shell becomes more flexible through weeks and months — when the time is ripe, hand pressure is
> enough, the shell opens like a perfectly ripened avocado! A different image came to me a few weeks
> ago. The unknown thing to be known appeared to me as some stretch of earth or hard marl, resisting
> penetration ... the sea advances insensibly in silence, nothing seems to happen, nothing moves, the
> water is so far off you hardly hear it ... yet it finally surrounds the resistant substance."

**VERBATIM (Grothendieck, R&S p. 555, trans. McLarty):** in the rising sea the theorem is "submerged
and dissolved by some more or less vast theory, going well beyond the results originally to be
established." Translation note: "rising sea" = **"la mer qui monte"** (McLarty fn.2). Deligne's
witness to the same style — **VERBATIM (Deligne 1998, p.12, via McLarty):** a characteristic
Grothendieck proof is "a long series of trivial steps where nothing seems to happen, and yet at the
end a highly non-trivial theorem is there." Grothendieck cast Serre as the opposite pole — Serre
"generally uses the hammer and chisel," is his "Super Yang" and the "incarnation of elegance"
(R&S, via McLarty).

**The engine, concretely.** He replaced objects with the *relations among all such objects*. A single
sheaf became, in his hands, a "meter stick" measuring a space; the object of study became the whole
category of them (McLarty). **VERBATIM (Cartier, *Inference*):** "His whole scientific strategy was,
indeed, organized around a progression of increasingly general concepts," and "Grothendieck's genius
consisted in solving the problem **from above**." The credo — **VERBATIM (Cartier):** "if one could
sufficiently penetrate its conceptual essence, then particular problems would be nothing but tests
that no longer need to be solved for their own sake." He called himself a "builder of cathedrals."

**Documented work volume.** Permanent professor at IHÉS 1958–1970 — "twelve years of undisputed
scientific reign" (Cartier). **VERBATIM (Cartier):** seminar sessions of "mathematical discovery, in
sessions lasting from ten to twelve hours!"; "Every day, he sent interminable and illegible
mathematical *feuilletons* to Dieudonné." The sustained-abstraction capacity was real and industrial:
EGA/SGA ran to thousands of pages of collaborative theory.

**The boundary lesson — where the sea did not rise (get this right; it is the anti-pattern).**
Grothendieck's plan for the **Weil conjectures** was to build the "right" cohomology and certify it via
his **standard conjectures on algebraic cycles** — then the Riemann-hypothesis analogue would follow
as pure theory. **The standard conjectures remain OPEN to this day** (Wikipedia, *Weil conjectures*,
VERBATIM: "Grothendieck's standard conjectures remain open (except for the hard Lefschetz theorem,
which was proved by Deligne ...)"). In **1974 Deligne proved the RH analogue anyway** — **VERBATIM
(Wikipedia):** "using the étale cohomology theory but **circumventing the use of standard conjectures
by an ingenious argument**." Deligne's route was a directed attack (a boundedness trick via Rankin,
Lefschetz pencils), *not* the theory Grothendieck wanted to see rise. Grothendieck's documented
reaction — **PARAPHRASE (grothendieckcircle "Spirituality" ch.10 / secondary):** he was "both
fascinated and disappointed"; "Deligne's proof was very different from what he had imagined." *Lesson
for the Ledger:* the rising sea has a failure mode — sometimes the water never covers the last rock,
and a "dirty," directed cut finishes the job the beautiful theory could not. Generality is a bet, not
a guarantee; a method that only ever refuses the head-on attack can be beaten to the theorem by one
who takes it.

**Genuine tension with the Euler Method (do not paper over it).** Grothendieck is the *anti-*compute-
first. Euler dwelt on tables of specific values; Grothendieck held that "particular problems ... no
longer need to be solved for their own sake." The transplant below is the *complement* to the Euler
loop, not an instance of it — it is what you reach for when the concrete assault has stalled and the
question is "what is the right category in which this is obvious?"

---

## 3. RICHARD FEYNMAN — what I cannot create, I do not understand

(Physicist, included because his METHOD is documented and it directly ratifies the plugin's
reconstruction-test doctrine.)

**The blackboard — VERBATIM (Caltech Archives photograph, Feynman's office board at his death,
15 February 1988).** Two mottos, in his own hand:
> "What I cannot create, I do not understand."
> "Know how to solve every problem that has been solved."

The first is the plugin's **reconstruction test** stated by another master: understanding is the
ability to *rebuild*, not to recognize. The second is its working corollary — a stocked internal
library of solved problems you can re-derive on demand. (Attestation is a photo of his board, not a
published aphorism — cite it as such; see folklore flag.)

**Redoing derivations from scratch — PARAPHRASE (Gleick, *Genius*, 1992).** Feynman read a paper only
until he grasped the problem, then closed it and worked the result out himself. Gleick's documented
consequence, and its cost: a physicist "who accumulated knowledge without taking the trouble to
publish could be a genuine danger to his colleagues" — others learned their career-making result had
been, to Feynman, "below the threshold of publishability." *Engine:* re-derivation is not
inefficiency; it is the calibration step that makes a result *yours* and exposes whether you actually
understand each link. This is Euler's **multi-route verification** and **re-derive-for-elegance** in a
physicist's key. *Anti-pattern honesty:* the same disdain for the literature is a documented cost —
re-deriving the known burns time and occasionally re-proves what was already in print.

**The twelve favorite problems — ATTRIBUTION PINNED.** This is **Rota reporting Feynman**, not Feynman
verbatim. **VERBATIM (Gian-Carlo Rota, "Ten Lessons I Wish I Had Been Taught," Notices AMS 44:1, Jan
1997):**
> "Richard Feynman was fond of giving the following advice on how to be a genius. You have to keep a
> dozen of your favorite problems constantly present in your mind, although by and large they will lay
> in a dormant state. Every time you hear or read a new trick or a new result, test it against each of
> your twelve problems to see whether it helps. Every once in a while there will be a hit, and people
> will say: 'How did he do it? He must be a genius!'"

Direct tie to Euler's **serial return** (Weil: Euler "never abandons a research topic ... he returns
to it, relentlessly") — but sharpened into a *filter*: every new tool is immediately tested against a
standing set of open problems.

**Compute/demonstrate first, in public, cheaply — the O-ring.** Rogers Commission hearing, 11 February
1986. Feynman had requested a glass of ice water and brought an O-ring section clamped in a C-clamp.
**VERBATIM (Rogers Commission Report, vol. 4, p. 680; also Gleick p. 423):** "I took this stuff I got
out of your [O-ring] seal and I put it in ice water, and I discovered that when you put some pressure
on it for a while and then undo it it doesn't stretch back." He closed: *"I believe that has some
significance for our problem."* *Engine:* a thirty-second physical demonstration on a national stage
beat a paper full of NASA statistics — the **compute-first / show-the-instrument** move, done in
public and for pennies. Euler's Instrument rule (calibrate on a known case before the reading counts)
has the same shape: the ice water *is* the calibrated experiment.

---

## 4. TERENCE TAO — the post-rigorous stage (primary source, living)

Tao's career-advice pages are a primary source for method written by a Fields medalist. Extracted
verbatim from terrytao.wordpress.com.

**The three stages — VERBATIM ("There's more to mathematics than rigour and proofs").** Pre-rigorous:
"mathematics is taught in an informal, intuitive manner, based on examples, fuzzy notions, and
hand-waving." Rigorous: "one is now taught that in order to do maths 'properly', one needs to work and
think in a much more precise and formal manner." **Post-rigorous:**
> "one has grown comfortable with all the rigorous foundations of one's chosen field, and is now ready
> to revisit and refine one's pre-rigorous intuition on the subject, but this time with the intuition
> solidly buttressed by rigorous theory."

And the load-bearing sentence — **VERBATIM:** "The point of rigour is not to destroy all intuition;
instead, it should be used to destroy bad intuition while clarifying and elevating good intuition."
→ This is the plugin's **understanding-over-storage** doctrine from the inside: mastery is *internalized*
rigor, at which point you may reason with the big picture because the formalism has become reflex — you
are re-deriving rigor on demand, not storing it.

**Compute-first, in his own words — PARAPHRASE/VERBATIM ("Solving mathematical problems").** He learned
from **Pólya's *How to Solve It*** at the Olympiads; his own book's first chapter names the concrete
tactics (try special/simple cases first; specialize then generalize; modify the problem; solve an
easier version) — the *try-simple-cases-first* move is Euler's **compute-first** exactly. And the
long-game — **VERBATIM:** "obtaining a solution is only the short-term goal of solving a mathematical
problem. The long-term goal is to increase your understanding." Comprehension test — **VERBATIM:** "if
you cannot adequately explain the solution of a problem to a classmate, then you haven't really
understood the solution yourself" (the reconstruction/Princess-gate test).

**Debunking the effortless-genius myth — VERBATIM ("Does one have to be a genius to do maths?").** "The
answer is an emphatic **NO**." "one does **not** need some sort of magic 'genius gene' that
spontaneously generates *ex nihilo* deep insights." He names the myth's cost: obsession with "big
problems"; skills that "stagnate" when solutions come too easily; others "too discouraged to continue."
From "Work hard" — **VERBATIM:** "mathematical breakthroughs are not powered solely (or even primarily)
by 'Eureka' moments of genius, but are in fact largely a product of hard work, directed of course by
experience and intuition," and "there is no royal road to mathematics." *Engine:* Tao converts Euler's
work-as-need from a temperament into a **stated discipline** — the post-rigorous stage is *earned* by
sustained effort, not conferred by talent.

---

## 5. FOLKLORE FLAGS (for the plugin's folklore firewall)

1. **"A mathematician is a machine for turning coffee into theorems" — NOT Erdős. It is Alfréd Rényi's
   line.** Earliest traceable attestation is Erdős himself crediting Rényi — **VERBATIM (Erdős, "Child
   Prodigies," 1971):** "In Hungary, many mathematicians drink strong coffee, in fact Rényi once said:
   a mathematician is a machine which turns coffee into theorems." Quote Investigator's verdict: Rényi
   is "the most likely creator," Erdős "the most significant popularizer," and it is now widely
   misattributed to Erdős. Secondary complication: Paul Turán's quip that weak coffee is "fit only for
   lemmas" (Dictionary of Scientific Biography). **Do not attribute the coffee line to Erdős.**

2. **Feynman's "What I cannot create, I do not understand" is a note on his death-day blackboard, not a
   published aphorism.** Attestation is the Caltech Archives photo (15 Feb 1988) — genuine and
   first-hand, but it is a note-to-self, undated as to composition, and people occasionally graft a
   Wittgenstein/first-principles genealogy onto it that has no primary basis. Quote the board; don't
   invent a lineage.

3. **The "twelve favorite problems" is Rota's report of Feynman, not a Feynman quotation.** No Feynman
   text says it in the first person; it lives in Rota's *Ten Lessons* (1997). Cite it as "Rota,
   reporting Feynman."

4. **Grothendieck "rising sea" translations are McLarty's own** (he states this, fn.1) — the vivid
   "ripened avocado" / "hard marl" wording is McLarty rendering "la mer qui monte." A different English
   translation of *Récoltes et Semailles* will phrase it differently; name the translator when quoting.

5. **Erdős coauthor count drifts (509 / 511 / 512).** The number depends on the counting date and
   whether posthumous joint papers are included. The mission's "511" is a commonly-cited figure; state
   it as approximate, not exact.

6. **The Weil-conjectures "boundary lesson" must not be flattened into "Grothendieck failed."** He did
   not: étale cohomology (his machine) is what Deligne's proof runs on. The precise, defensible claim
   is narrower — Grothendieck's *intended route* (via the standard conjectures) was not the one that
   closed the problem, the standard conjectures are still open, and he was documented as disappointed
   that the finish was a directed argument rather than the rising tide he wanted. Keep it that precise.

---

## 6. TRANSFERABLE MOVES (per figure, with receipts)

**ERDŐS**
- *Price the difficulty.* State, out loud, how far past your current tools a problem sits — as if
  setting a bounty ("this is a $25 step; that is a $10,000 step"). The estimate is information and it
  ranks where to spend effort. (Receipt: Graham/Quanta, "$25 problem or possibly a $100 problem.")
- *Be the router.* Hold many open problems and many solvers in one place and make the matches; a
  problem handed to the right mind beats a problem hoarded. (Receipt: Babai — "catalyst of interaction
  ... making introductions"; ~511 coauthors.)
- *Let elegance be the compass.* Rank a proof by whether it is "from The Book," and keep hunting a
  clumsy proof for its Book version. (Receipt: Aigner–Ziegler preface; ties to Euler re-derive-for-
  elegance.)

**GROTHENDIECK**
- *Solve from above.* When the head-on assault stalls, stop hammering and ask "in what more general
  setting is this theorem obvious?" — then build that setting. (Receipt: Cartier, "solving the problem
  from above"; the rising-sea passage.)
- *Turn the object into the category of objects.* Study not the thing but the system of all such
  things and their maps (the "meter stick" move). (Receipt: McLarty on sheaves-as-meter-sticks.)
- *Know the boundary: generality is a bet.* Before committing to build the whole theory, ask whether a
  directed cut might finish faster — the standard conjectures are still open and Deligne won by
  circumventing them. (Receipt: Wikipedia, *Weil conjectures*; the disappointment record.)

**FEYNMAN**
- *The creation test.* For anything you claim to understand, try to re-derive it from a blank page; if
  you cannot build it, you do not understand it. (Receipt: the blackboard, Caltech Archives — this IS
  the plugin's reconstruction test, independently arrived at.)
- *Keep a standing set of ~12 open problems and test every new tool against all of them.* (Receipt:
  Rota, *Ten Lessons* — reporting Feynman.)
- *Demonstrate first, cheaply, in public.* When the argument is contested, build the smallest physical
  or computational demonstration that settles it and show it. (Receipt: O-ring in ice water, Rogers
  Commission vol. 4 p. 680.)

**TAO**
- *Aim for the post-rigorous stage — and know it must be earned.* Internalize the rigor until you can
  reason with the big picture; do not skip the rigorous stage to get there. (Receipt: "There's more to
  mathematics than rigour and proofs," verbatim.)
- *Try the simplest special case first.* Named explicitly among his problem-solving tactics; identical
  to Euler compute-first. (Receipt: "Solving mathematical problems"; Pólya lineage.)
- *Treat the effort as the method, not a fallback.* "There is no royal road"; breakthroughs are "hard
  work, directed by experience and intuition," not Eureka. (Receipt: "Work hard" and "Does one have to
  be a genius to do maths?", verbatim.)

---

## Sources actually read (URLs)

- McLarty, *The Rising Sea: Grothendieck on Simplicity and Generality* (PDF, translations his own):
  https://www.landsburg.com/grothendieck/mclarty1.pdf
- nLab, *The Rising Sea* (rising-sea passage, cites R&S pp. 552-3): https://ncatlab.org/nlab/show/The+Rising+Sea
- Cartier, *A Country Known Only by Name* (Grothendieck memoir), *Inference*:
  https://inference-review.com/article/a-country-known-only-by-name
- Wikipedia, *Weil conjectures* (Deligne circumventing the standard conjectures):
  https://en.wikipedia.org/wiki/Weil_conjectures
- Grothendieck Circle, "Spirituality" ch.10, *The Weil Conjectures* (Grothendieck's reaction):
  https://webusers.imj-prg.fr/~leila.schneps/grothendieckcircle/Spirituality/Spirituality10.pdf
- AMS, *The Life of Grothendieck* (part 2): https://www.ams.org/notices/200410/fea-grothendieck-part2.pdf
- Gowers, *The Two Cultures of Mathematics* (PDF, read in full):
  https://www.dpmms.cam.ac.uk/~wtg10/2cultures.pdf
- Babai, *In and Out of Hungary: Paul Erdős, His Friends, and Times* (PDF, read):
  http://people.cs.uchicago.edu/~laci/erdos80.pdf
- Quanta, *Cash for Math: The Erdős Prizes Live On* (2017), Graham on pricing:
  https://www.quantamagazine.org/cash-for-math-the-erdos-prizes-live-on-20170605/
- Quanta, *In Search of God's Perfect Proofs* (2018), Aigner–Ziegler / "The Book":
  https://www.quantamagazine.org/gunter-ziegler-and-martin-aigner-seek-gods-perfect-math-proofs-20180319/
- Wikipedia, *Proofs from THE BOOK* (Erdős 1985 "believe in The Book"):
  https://en.wikipedia.org/wiki/Proofs_from_THE_BOOK
- Quote Investigator, *A Mathematician Is a Machine Which Turns Coffee into Theorems* (Rényi origin):
  https://quoteinvestigator.com/2026/06/13/mathematician-coffee/
- Tao, *There's more to mathematics than rigour and proofs*:
  https://terrytao.wordpress.com/career-advice/theres-more-to-mathematics-than-rigour-and-proofs/
- Tao, *Solving mathematical problems*: https://terrytao.wordpress.com/career-advice/solving-mathematical-problems/
- Tao, *Does one have to be a genius to do maths?*:
  https://terrytao.wordpress.com/career-advice/does-one-have-to-be-a-genius-to-do-maths/
- Tao, *Work hard*: https://terrytao.wordpress.com/career-advice/work-hard/
- Rota, *Ten Lessons I Wish I Had Been Taught*, Notices AMS 44:1 (1997) — verbatim via fs.blog:
  https://fs.blog/gian-carlo-rota/ • AMS PDF (403 this session): https://www.ams.org/notices/199701/comm-rota.pdf
- Feynman blackboard, Caltech Archives (15 Feb 1988), via Paul Halpern / samim.io:
  https://samim.io/p/2025-02-21-richard-feynmans-blackboard-at-time-of-his-death-his/
- Feynman O-ring testimony, Rogers Commission vol. 4 p. 680 — via libquotes + Gleick p. 423:
  https://libquotes.com/richard-feynman/quote/lbt6e2j • http://feynman.com/science/the-challenger-disaster/
- Gleick, *Genius* (Feynman re-deriving / disregard for literature), via search of Wikiquote + Marginalian:
  https://en.wikiquote.org/wiki/Richard_Feynman
