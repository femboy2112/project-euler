# Project EULER

> *observation · daring guess · shrewd verification*

A Leonhard Euler mathematical-method discipline for Claude Code — built on the thesis that
Euler's **method** did an un-insignificant portion of the work his genius gets credit for, and
that the method is transplantable. This wiki documents the method with receipts; the plugin
turns it into an operating discipline.

## The thesis, in one paragraph

Pólya's verdict on Euler: he made his discoveries "by induction, that is, by observation, daring
guess, and shrewd verification" — and he is "almost unique in one respect: he takes pains to
present the relevant inductive evidence carefully, in detail, in good order... honestly, as a
genuine scientist should do." That second sentence is why this plugin can exist: of all the
great mathematicians, Euler is the one whose *process* is documented, because he published it —
false starts included. What is documented can be studied; what can be studied can be practiced.

## The pages

- **[The-Method](The-Method.md)** — the seven moves, each anchored to a verified historical
  episode (E-numbers and all).
- **[The-Engine](The-Engine.md)** — what was underneath the moves: the intrinsic-drive
  hypothesis, tested against the primary record, and how the plugin operationalizes it.
- **[The-Ledger](The-Ledger.md)** — the epistemic labels, in Euler's own dialect.
- **[The-Iron-Rule](The-Iron-Rule.md)** — why the persona is safe: the voice rides the prose,
  the facts stay exact.
- **[The-Masters](The-Masters.md)** — the masters' wing: Ramanujan, Gauss, Newton, Poincaré,
  Hadamard, Erdős, Grothendieck, Feynman, Tao — each unique skillset distilled into general
  form, with receipts and boundary lessons.
- **[The-Cast](The-Cast.md)** — the twelve members of the Academy and what each is for.
- **[Folklore-Firewall](Folklore-Firewall.md)** — the debunked anecdotes this plugin refuses to
  repeat as fact, with the debunking receipts.
- **[Session-Modes](Session-Modes.md)** — /euler-mode, /academy, /opera, and the one-shots.
- **[FAQ](FAQ.md)**

## The receipts

Everything historical in this plugin traces to the nine research dossiers in
[`research/`](../research/). Dossiers I–IV are the Euler study — compiled from primary and
scholarly sources (Pólya's *Mathematics and Plausible Reasoning* read in scan, the 1783 Fuss
and Condorcet eulogies in English and French, 15 of Ed Sandifer's "How Euler Did It" columns,
Bell's translations of E41 and the Goldbach correspondence, Weil, Varadarajan, Lagarias,
Gautschi, Lemmermeyer, Aycock). Dossiers V–VIII are the masters' wing — Ramanujan (Hardy's
*Twelve Lectures*, Littlewood, Berndt), Gauss and Newton (the Encke letter, the Tagebuch, the
Newton Project manuscripts), Poincaré and Hadamard (*Mathematical Creation* read in the primary
Halsted printing), and the moderns (Gowers, McLarty, Cartier, Rota, the Rogers Commission
transcript, Tao's own advice pages). Dossier IX — the Poincaré–Hadamard *generative methods*
report, supplied by the Correspondent — powers the `poincare` and `hadamard` agents; its
provenance header maps its own evidence discipline onto the house labels. Every claim is
labeled VERBATIM / PARAPHRASE / LEGEND-UNVERIFIED with its source stated. The plugin holds
itself to its own Ledger.

## Install

```
/plugin marketplace add <path-or-repo>       # e.g. /home/leah/ProjectEULER
/plugin install project-euler@project-euler
```

Then `/euler-mode` — and the correspondence begins.
