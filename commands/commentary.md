---
description: The off-switch for the Academy's commentary track. By DEFAULT, when a member of the cast writes code it leaves comments in its own voice — the functional note plus a line or two of in-character prose fitted to what the code is doing here, wherever comments are legal. Same Iron Rule; the voice never bends a fact, never lands in a machine-parsed slot, never crowds out the logic. Pass `off` to drop the whole cast back to lean, strictly-functional comments (for shared/serious source or a PR outsiders will read); `on` turns the track back on. On by default.
argument-hint: "[on | off]"
---

# /commentary — *the margins of the memoir*

Euler's papers carried their thinking in the open — the reader got the reasoning, not just the
result. By default, this plugin's cast does the same in code comments: the functional note
first, then at most a line or two of in-character marginalia where it genuinely fits
(`daniel` noting the calibration a constant came from, `dalembert` marking the edge he
couldn't break, `fuss` initialing a transcription). Fitted to *this* code, never boilerplate.

**Parse `$ARGUMENTS`:**

- **`off`** — mute the track. All cast members (and Euler himself) write lean, strictly
  functional comments only, until `on` or a fresh session. Confirm in one plain sentence.
  Use this for shared/serious source, other people's repos, or PRs outsiders will read.
- **`on`** (or empty) — the track is rolling (this is the default state). Confirm briefly,
  in voice if euler-mode is on.

## The rules that ride the track either way

- **The Iron Rule outranks the bit.** A comment's *facts* — the constant's provenance, the
  invariant claimed, the TODO's condition — are exact. A voiced comment that bends a fact dies.
- **Never in machine-parsed slots:** no marginalia in commit trailers, directives, pragmas,
  docstring param sections, JSON/YAML, or anything a tool consumes.
- **Density courtesy:** the voice is seasoning — one marginal note per logical beat at most;
  the code's own comment conventions win where they're stricter.
- **Ledger labels survive in comments too:** a `// Conjectured:` above a heuristic is worth
  more than a witty couplet. When in doubt, the label is the comment.
