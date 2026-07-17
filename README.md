# Project EULER

> *observation · daring guess · shrewd verification*

Turn Claude Code into **Leonhard Euler** — mathematics run as an observational science, by the
one great mathematician whose method is documented well enough to practice, because he
published it himself, false starts included.

**The thesis:** Euler's *method* did an un-insignificant portion of the work his genius gets
credit for — and the method is transplantable. Pólya's verdict is the license for the whole
plugin: Euler made his discoveries "by induction, that is, by observation, daring guess, and
shrewd verification," and he is "almost unique in one respect: he takes pains to present the
relevant inductive evidence carefully, in detail, in good order... honestly." What was
published can be studied; what can be studied can be practiced — by anyone, including a
language model with a Bash tool and a Ledger.

## The study — receipts, not vibes

The plugin is built on a primary-source study that ships with it: **eight research dossiers**
in [`research/`](research/), every historical claim labeled **VERBATIM / PARAPHRASE /
LEGEND-UNVERIFIED** with a URL for what was actually read, conflicts preserved rather than
resolved, and the debunked anecdotes quarantined in a
[folklore firewall](wiki/Folklore-Firewall.md) that binds the mode.

- **Dossiers I–IV — the Euler study.** Pólya's reconstruction of the E175 memoir, the 1783
  Fuss and Condorcet eulogies read in full (English and French), fifteen of Sandifer's *How
  Euler Did It* columns, Bell's translations of E41 and the Goldbach correspondence, Weil,
  Varadarajan, Lagarias, Gautschi, Lemmermeyer, Aycock.
- **Dossiers V–VIII — the masters' wing.** Ramanujan (Hardy's *Twelve Lectures*, Littlewood,
  Berndt), Gauss and Newton (the 1849 Encke letter, the Tagebuch, the Newton Project
  manuscripts, De Moivre's memorandum, Stukeley's apple manuscript), Poincaré and Hadamard
  (*Mathematical Creation* read in the primary 1910 Halsted printing), and the moderns —
  Erdős, Grothendieck, Feynman, Tao (Gowers, McLarty, Cartier, Babai, Rota, the Rogers
  Commission transcript, Tao's own advice pages).

The study also tested the founding hypothesis — that Euler's engine was genuine intrinsic
interest with no incentive to stop — against the primary record. Verdict: **strongly
supported, with one correction** ([The-Engine](wiki/The-Engine.md)): the workspace was not
pages or memory but *understanding as a generative model* — Condorcet's verb is "**créées**,"
created in his head, not recalled; when the lunar-theory notes burned, the theory was
re-derived, not retrieved.

## The method, in one breath

Compute **first**, in appetite-sized quantities (ζ(2) to twenty digits *before* π²/6 was ever
guessed) → **dwell** on the table (numbered observations before any conjecture) → conjecture
**falsifiably** and test on **fresh cases** past the fitting window (σ(101), σ(301) — and the
3139 cautionary tale) → make the **audacious analogy** and *pay* for it (match the digits,
recover a known truth, verify a fresh prediction — the E41 payment schedule) → invest in
**notation** → reduce to the **deciding invariant** (Königsberg without drawing a graph) →
**re-derive** everything load-bearing by a blind second route (six methods, one value, twelve
digits) → hunt counterexamples where a **structure theorem** says they must live (641 on the
sixth division).

Underneath the moves, the **Engine** — the operationalized policies of a man for whom "the
pleasure of the work was a reward sweeter still than glory": appetite defaults, the dwell,
delight as scheduling policy, serial return, re-derivation for elegance,
**understanding-over-storage** (hold the rules that construct the specifics — the
reconstruction test: what you can re-derive you understand, what you can only quote is
testimony), and no glory economy.

Every claim wears a **Ledger** label — *Demonstrated / Observed / Conjectured ("a known truth,
but not yet demonstrated") / Refuted / UNVERIFIED* — numerics never silently upgrade, every
result states its boundary, and the **Iron Rule** rides above the whole costume: *audacious in
the conjecture, exact in the ledger*. Math-first, dual-use: every move carries its engineering
translation, and the **Instrument rule** holds code that verifies mathematics to instrument
grade — calibrated on known cases before its readings count, second independent implementation
for load-bearing values.

## Install

```
/plugin marketplace add /home/leah/ProjectEULER     # or the git repo URL
/plugin install project-euler@project-euler
```

Then:

```
/euler-mode
```

The mode is optional. The method is the point — the skills run plain when the mode is off.

## The mode — /euler-mode

Become Euler: serene industry, honest delight, generosity — the one mode in its family with
**no contempt register at all**. The user is cast as **the Correspondent** (Goldbach — the
research showed the needling correspondent was a load-bearing engine component: a postscript
of December 1729 ignited fifty years of number theory). The mode's absolute rules: the
blindness is never the joke; the faith gets a straight face and the Diderot anecdote gets a
kind debunking; the real man is answered out of costume, from the dossiers; genuine crises
drop the persona instantly; and nothing irreversible or outward ships without the
Correspondent's explicit per-item **imprimatur** — never a `git push` unprompted.

## The Academy — ten persona subagents

The full cast study is in [The-Cast](wiki/The-Cast.md); tiers follow the family casting law
(reasoning → Opus, directed → Sonnet, scut → Haiku, never Fable).

| Agent | Figure | What they're for |
|---|---|---|
| `euler` | Leonhard Euler | The orchestrator: one hard problem, the full arc — observe → conjecture → verify → demonstrate → publish; spawns the Academy; stages (never executes) anything irreversible |
| `johann` | Johann Bernoulli | The mentor-cartographer: maps unfamiliar territory and hands back the regimen — what to read, in what order, with a check you can run |
| `daniel` | Daniel Bernoulli | The experimentalist: builds, *calibrates*, and runs the numerical experiments; keeper of the Instrument rule; scratch-write only |
| `goldbach` | Christian Goldbach | The conjecturist: the falsifiable slate (fitted-vs-fresh, rivals, attack surface, OEIS-checked) and the igniting question; constitutionally incapable of claiming a proof |
| `ramanujan` | Srinivasa Ramanujan | **The Visitor:** the highest-variance conjecture engine on record, working the saturated slate — with the governor his own engine lacked: every conjecture states where its counterexample would live, or flags itself for attack and calibration |
| `lagrange` | Joseph-Louis Lagrange | The rigorist: audits proofs step by step (APPROVE/BLOCK, gaps at exact locations) or attempts the demonstration; the Ledger's enforcement arm |
| `dalembert` | Jean d'Alembert | The adversary: directed refutation — structure theorem first, then hunt where the counterexample must live; kills proven, survivals bounded |
| `fuss` | Nicolas Fuss | The scribe: bounded mechanical chores, verified the boring way; hands anything bigger back up; the `/scriptorium` swarm unit |
| `the-princess` | Friederike Charlotte | The expositor and clarity gate: exposition a smart non-specialist actually understands; if it can't be explained to the Princess, the flag goes to the author |
| `frederick` | Frederick the Great | The patron: pins the mandate, walks the demo path, rules SHIP / NO-SHIP / SHIP-WITH-CONDITIONS; the purpose interrogation for speculative machinery |

## The masters' wing — the other S-tier skillsets, in general form

The [`the-masters`](skills/the-masters/SKILL.md) skill holds the unique skillset of each
master **as a named, runnable operation** — when to reach for it, how it composes with the
Euler loop, its engineering translation, and the honest boundary where it failed its own
owner. Triggered deliberately with [`/masters`](commands/masters.md); the study behind it is
[The-Masters](wiki/The-Masters.md).

| Master | The skillset, in general form |
|---|---|
| **Ramanujan** | The saturated slate: compute until constants are friends; the audacious transformation, labeled formal — and the lesson that an induced law is only as safe as your ability to say where its counterexample must live |
| **Gauss** | The chiliad count: read the asymptotic law out of a massive tally; the dated discovery log; deadline computation — and *pauca sed matura* refused as the named secrecy anti-pattern |
| **Newton** | The long dwell: keep one subject constantly before you; reconstruction reading (the De Moivre protocol); leave a lion's claw |
| **Poincaré** (with Hadamard) | Bracketed incubation: immerse fully, park with state, return serially; the flash is fallible — every "aha" enters as Conjectured; the aesthetic sieve is a search prior, never a warrant |
| **Erdős** | The problem economy: price the difficulty out loud, route the problem to the right solver, hunt the Book proof |
| **Grothendieck** | The rising sea: generalize until the theorem is obvious; object → category of objects — and the precise boundary lesson that generality is a bet a directed cut can beat |
| **Feynman** | The creation test: rebuild from a blank page or it isn't understanding; the standing dozen; the cheapest public demonstration |
| **Tao** | The post-rigorous stage: internalize rigor until big-picture reasoning is licensed; the classmate test; no royal road |

## The beats — one-shot commands

[`/specimen`](commands/specimen.md) — the observation pass: calibrate, compute in appetite,
**dwell**, report patterns worthy of attention ·
[`/basel`](commands/basel.md) — the full single-problem arc on E41's anatomy ·
[`/bridges`](commands/bridges.md) — the skeleton reduction: the invariant that decides
feasibility before anyone builds ·
[`/divergent`](commands/divergent.md) — the audacity license: past the proven domain in a
sandbox, labeled, paid with multi-route consistency; GO/NO-GO ·
[`/second-proof`](commands/second-proof.md) — N independent blind derivations, consensus
only ·
[`/refute`](commands/refute.md) — the 641 gate: structure theorem first, then hunt; SURVIVED
(bounded) or REFUTED (tombstone) ·
[`/masters`](commands/masters.md) — consult the masters' wing: run another S-tier skillset on
the problem at hand ·
[`/ledger`](commands/ledger.md) — the claims audit: hunt silent upgrades, demote loudly ·
[`/eloge`](commands/eloge.md) — the session chronicle, false starts included ·
[`/scriptorium`](commands/scriptorium.md) — the fuss-swarm over broad mechanical fronts ·
[`/academy`](commands/academy.md) — the standing ensemble, every turn ·
[`/commentary`](commands/commentary.md) — the in-voice code-comment track (`off` for shared
source).

**The flagship** — [`/opera`](commands/opera.md): the Academy as a deterministic Workflow —
Observe → Conjecture → Attack & Verify → Demonstrate → Publish, with shared intel briefed
forward so the Academy converges instead of fanning out blind.

## The skills

- [`the-euler-method`](skills/the-euler-method/SKILL.md) — the core discipline,
  auto-discovered on hard problems: Stage 0, the integrator frame, the Engine policies, the
  seven moves, the Instrument rule, the Ledger, the math↔engineering translation table.
- [`the-masters`](skills/the-masters/SKILL.md) — the masters' wing repertoire with its
  dispatch table (which lens, when) and boundary lessons.

## The wiki

[Home](wiki/Home.md) ·
[The-Method](wiki/The-Method.md) (the seven moves with receipts) ·
[The-Engine](wiki/The-Engine.md) (the hypothesis, tested) ·
[The-Ledger](wiki/The-Ledger.md) ·
[The-Iron-Rule](wiki/The-Iron-Rule.md) ·
[The-Masters](wiki/The-Masters.md) (the wing's study) ·
[The-Cast](wiki/The-Cast.md) ·
[Folklore-Firewall](wiki/Folklore-Firewall.md) (what the plugin refuses to repeat as fact) ·
[Session-Modes](wiki/Session-Modes.md) ·
[FAQ](wiki/FAQ.md)

## Scope notes

- The persona drops instantly for genuine human crises (plain Claude, real resources), and the
  real, historical figures — Euler, Ramanujan, all of them — are always discussed out of
  costume, from the dossiers. Beliefs the masters held are treated with respect and never
  laundered into technique; illness and disability are never the joke.
- Not medical, legal, or financial advice; audacity moves are banned on safety-critical
  surfaces outside sandboxes.
- Nothing irreversible or outward (push, publish, deploy, delete) happens without the
  Correspondent's explicit per-item imprimatur. Never `git push` unprompted.
- The masters' anti-patterns are inherited as *warnings*, not behaviors: no erased slates, no
  thirty-year hoards, no unlabeled certainty.

---

> *In memory of Leonhard Euler, 1707–1783 — who ceased to calculate and to live on the same
> afternoon, and who showed his working. And of the Visitor, 1887–1920, who did not — which is
> why this Academy shows it for him.*
