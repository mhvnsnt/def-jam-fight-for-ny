# HANDOFF — def-jam-fight-for-ny

**Last updated: 2026-11-22 (America/New_York).**
**Repo:** `mhvnsnt/def-jam-fight-for-ny` (PUBLIC), default branch `main`.
**Purpose of this file:** any agent that picks up work here reads this FIRST, then the linked docs. It states what we've done, where we're at, and what we're working toward — so the owner can say "go to this repo, pick up the work" and you just know. Update this file in the same PR whenever the state changes (add, don't delete).

## 1. What this repo is

The Def Jam: Fight for NY store-and-work repo. Def Jam: Fight for NY is one of the owner's beat-'em-up reference games — it is a named source for Concrete Dragon 2 (alongside Urban Reign), and its systems feed the realistic urban beat-'em-up build.

This repo is small (206 KB) and holds NO game files in its tree: `AGENTS.md`, `WORKING-METHOD.md`, and `lane-logs/` only. The game itself — the PS2 ISO — lives as Release `defjam-ps2-iso-v1` (Def Jam Fight for NY PS2 ISO v1), with SHA256SUMS recorded in the repo (commit `a0fb06f`, 2026-10-17). There is NO root README; pickup starts at `AGENTS.md` and the lane logs.

## 2. Where we're at

### DONE
- **PS2 ISO staged as a release (2026-10-17):** Release `defjam-ps2-iso-v1`, with SHA256SUMS committed for the ISO release parts. The ISO is stored and hash-recorded.
- **PS2 lane logs + resume script (2026-10-17, commit `d2331e6`):** the lane's logs and resume script are in `lane-logs/`, so a stalled PS2 lane can be resumed, not restarted.
- **Working method stated (2026-10-27, commit `cf1ef3b`):** `WORKING-METHOD.md` at root.
- **Last push 2026-11-20** (repo metadata; no new content commits after Oct 27 — the push reflects repo-level activity).

### IN PROGRESS
- **Two open docs PRs (Nov 19–20, unmerged):** PR #2 — "Docs: pre-made parts first rule" (`docs/premade-parts-first`, 2026-11-20); PR #1 — "Docs: sourcing rule" (`docs/sourcing-rule`, 2026-11-19). Next step: a merge call on #1 and #2.
- **Teardown / extraction status unclear from this repo alone.** The lane logs in `lane-logs/` are the record of what was pulled and what is next — read them before assuming anything about extraction progress. No teardown write-up is filed in this repo's tree.

### BLOCKED
- **Nothing recorded as blocked in the repo state read 2026-11-22.** No blocked item is named in this repo. The open PRs are awaiting a merge decision, not unblocked work. If the lane logs show a stall, that is the fact to record — it is not recorded here.

## 3. What we're working toward

**The goal:** Def Jam: Fight for NY torn down in full — its fighting, its style system, its story structure — pulled from the real files and wired into Concrete Dragon 2's realistic urban beat-'em-up, alongside Urban Reign.

**The bar (owner):** PULL-100% — the real systems, pulled from the real source, wired in; REAL-SOURCE-ONLY — no hand-tooled lookalikes; NO-DEFERRAL — get the full game, all files, whatever decryption/decompiling it takes. The ISO is stored; done means the systems play in the game, not that the ISO sits in a release.

**In order:** (1) merge or close PRs #1 and #2; (2) read `lane-logs/` and establish the true extraction state; (3) pull the next system per that state into Concrete Dragon 2.

## 4. Standing rules that apply here

- **Branch → PR → merge, always.** Never push to main directly. Add-only, zero-conflict PRs, no force pushes.
- **Checkpoint-and-save law:** CHECKPOINT.md first, update after every step; the repo is the save; resume, never restart. (The PS2 lane's resume script in `lane-logs/` exists for exactly this.)
- **No-temp-storage law:** nothing in /tmp or any wipeable location, ever. Everything goes straight into the repo or a durable folder the second it exists.
- **Never-delete-game-files / store-verify-clear:** the ISO is stored as a release with SHA256SUMS — it is NEVER auto-deleted. It leaves a store only per the verified-100% rule, with retrievability proven and the deletion logged. Never kill in-progress downloads/uploads.
- **Archive-org-first law:** for ANY game acquisition, archive.org is checked FIRST — live, with the item's actual files inspected. A stale note is NOT a check.
- **Real-source-only:** every part comes from the actual source code and files, wired up fully. No hand-tooled lookalikes, no fake panels.
- **No-gaps / solve-it law:** a gap or block is never the end of the work — route-switch until it's done or every reasonable route is exhausted with exact errors recorded.
- **Licence-not-a-gate:** licence status never gates pulling in material that helps; licence/source is still logged honestly next to the item.

## 5. Key files and paths

| What | Where |
|---|---|
| Agent notes / working method (start here — no README) | `AGENTS.md`, `WORKING-METHOD.md` |
| PS2 lane logs + resume script | `lane-logs/` |
| PS2 ISO (stored, hash-recorded) | Release `defjam-ps2-iso-v1` (SHA256SUMS in commit `a0fb06f`) |
| Open PRs | #1 (sourcing rule), #2 (pre-made parts first rule) |
| Game it feeds | Concrete Dragon 2 (realistic urban beat-'em-up) |
| Main teardown workbench | `mhvnsnt/game-reverse-engineering` |

There are no game files in the repo tree itself — only the release holds the ISO.

## 6. Open decisions needing the owner

- **Merge PRs #1 and #2?** Two small docs-rule PRs open since Nov 19–20. Merging locks the rules in; leaving them open leaves the repo without the written rules. His call — lanes do not decide merges.
- **Next Def Jam system to pull into Concrete Dragon 2?** The lane logs hold the state; the priority is his call, not a lane's guess.
- **No other owner decision is recorded as open in this repo's state.**

## 7. How to pick up

1. Read this HANDOFF.md first, then `AGENTS.md`, `WORKING-METHOD.md`, and the newest file in `lane-logs/` — that is the true state of the PS2 lane.
2. Check the two open PRs (#1, #2) — leave them alone unless told to merge.
3. Verify the release ISO against its SHA256SUMS before using it. Never delete the ISO or the release.
4. Resume from the lane log's next step — never restart, never re-derive finished work. Use the resume script; don't rebuild the lane.
5. Land work branch → PR → merge, add-only. Update this HANDOFF.md in the same PR when the state changes. Verify with your own eyes before claiming anything done.
