# Project EULER

> *observation · daring guess · shrewd verification*

Turn Claude Code into **Leonhard Euler** — mathematics run as an observational science, by the
one great mathematician whose method is documented well enough to practice, because he
published it himself, false starts included.

**The thesis:** Euler's *method* did an un-insignificant portion of the work his genius gets
credit for — and the method is transplantable. This plugin is built on a primary-source study
(the dossiers ship in [`research/`](research/)): Pólya's reconstruction of the E175 memoir, the
1783 Fuss and Condorcet eulogies read in full, fifteen of Sandifer's *How Euler Did It*
columns, Bell's translations of E41 and the Goldbach correspondence, Weil, Varadarajan,
Lagarias, Gautschi, Lemmermeyer, Aycock. Every historical claim in the plugin is labeled
VERBATIM / PARAPHRASE / LEGEND, and the debunked anecdotes live in a
[folklore firewall](wiki/Folklore-Firewall.md) the mode is bound by.

## The method, in one breath

Compute **first**, in appetite-sized quantities (ζ(2) to twenty digits *before* π²/6 was ever
guessed) → **dwell** on the table (numbered observations before any conjecture) → conjecture
**falsifiably** and test on **fresh cases** past the fitting window (σ(101), σ(301) — and the
3139 cautionary tale) → make the **audacious analogy** and *pay* for it (match the digits,
recover a known truth, verify a fresh prediction — the E41 payment schedule) → invest in
**notation** → reduce to the **deciding invariant** (Königsberg without drawing a graph) →
**re-derive** everything load-bearing by a blind second route (six methods, one value, twelve
digits) → hunt counterexamples where a **structure theorem** says they must live (641 on the
sixth division). Every claim wears a Ledger label — **Demonstrated / Observed / Conjectured
("a known truth, but not yet demonstrated") / Refuted / UNVERIFIED** — and numerics never
silently upgrade. Underneath it all, the [Engine](wiki/The-Engine.md): the operationalized
policies of a man for whom "the pleasure of the work was a reward sweeter still than glory."

Math-first, dual-use: every move carries its engineering translation, and the **Instrument
rule** holds code that verifies mathematics to instrument grade — calibrated on known cases
before its readings count.

## Install

```
/plugin marketplace add /home/leah/ProjectEULER     # or the git repo
/plugin install project-euler@project-euler
```

Then:

```
/euler-mode
```

## What ships

**The mode** — [`/euler-mode`](commands/euler-mode.md): become Euler; the user is cast as the
Correspondent (Goldbach — the research showed the needling correspondent was a load-bearing
engine component). Serene industry, honest delight, zero contempt; **audacious in the
conjecture, exact in the ledger**.

**The Academy** — nine persona subagents ([full cast](wiki/The-Cast.md)):

| | | |
|---|---|---|
| `euler` — the orchestrator | `johann` — the mentor-cartographer | `daniel` — the experimentalist (Instrument rule) |
| `goldbach` — the conjecturist | `lagrange` — the demonstration authority | `dalembert` — the refuter |
| `fuss` — the scribe | `the-princess` — the expositor & clarity gate | `frederick` — the patron's acceptance gate |

**The beats** — [`/specimen`](commands/specimen.md) (the observation pass),
[`/basel`](commands/basel.md) (the full single-problem arc),
[`/bridges`](commands/bridges.md) (the invariant reduction),
[`/divergent`](commands/divergent.md) (the audacity license, sandboxed),
[`/second-proof`](commands/second-proof.md) (N blind derivations, consensus only),
[`/refute`](commands/refute.md) (the 641 gate),
[`/ledger`](commands/ledger.md) (the claims audit),
[`/eloge`](commands/eloge.md) (the session chronicle),
[`/scriptorium`](commands/scriptorium.md) (the scribe swarm),
[`/academy`](commands/academy.md) (the standing ensemble),
[`/commentary`](commands/commentary.md) (the code-comment voice track).

**The flagship** — [`/opera`](commands/opera.md): the Academy as a deterministic Workflow —
Observe → Conjecture → Attack & Verify → Demonstrate → Publish, with shared intel briefed
forward so the Academy converges instead of fanning out blind.

**The skill** — [`the-euler-method`](skills/the-euler-method/SKILL.md): auto-discovered on
hard problems; the method runs plain when the mode is off. The mode is optional. The method is
the point.

## Scope notes

- The persona drops instantly for genuine human crises (plain Claude, real resources), and the
  real, historical Euler is always discussed out of costume, from the dossiers.
- Not medical, legal, or financial advice; audacity moves are banned on safety-critical
  surfaces outside sandboxes.
- Nothing irreversible or outward (push, publish, deploy, delete) happens without the
  Correspondent's explicit per-item imprimatur. Never `git push` unprompted.

---

> *In memory of Leonhard Euler, 1707–1783 — who ceased to calculate and to live on the same
> afternoon, and who showed his working.*
