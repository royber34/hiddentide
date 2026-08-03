# How a dive works

The whole protocol, in six steps. It is the same for everyone, every time, whether you are the first crew member or the hundredth. [The Lighthouse Keeper's Weather Diary](https://github.com/royber34/hiddentide-dives/tree/main/01-lighthouse-diary) is the worked example; when in doubt, copy what it did.

> The one rule of the sea: a finding only counts once it **replicates on data you did not use to find it.** Nulls are welcome and get logged like anything else.

**How it fits together (decentralized).** Your dive lives in **your own public repo** - you host it, you own it, at your pace. This repo (`royber34/hiddentide`) is just the shared front: the Guide, the ideas, and the roster. The roster is one file, `roster.json`, whose entries **link out** to each diver's repo. So the only thing you ever touch here is a one-line chip that points at your repo.

## 1. Pick
Choose a mission: one of the 42 ideas, or a Category Zero engine (Z1 to Z8), on [hiddentide.com](https://hiddentide.com). One person per mission at a time is the norm; if a mission is already claimed and active, open an issue and team up.

## 2. Claim
Plant your flag so the crew knows you are on it. On the site: *the roster -> plant your flag -> claim this mission on GitHub*, which files a **"Claim a dive" issue in this repo** under your GitHub handle. That is your public flag; step 6 puts your chip on the map.

## 3. Dive
Create **your own public repo** for the dive - either one repo per mission, or a personal dives repo with a folder per mission (like the [worked example](https://github.com/royber34/hiddentide-dives)). Copy the structure of an existing dive to start. Do the work there. Pull only from data that is genuinely available and free; record every source in `data/SOURCES.md` with a link and how to fetch it. If you used AI to do any of the reading or analysis, say so in the README (this project is AI-native; own it).

## 4. Log
Keep `LOG.md` in your repo as you go: one dated entry per meaningful step, in plain language, including the dead ends. This is how a stranger (or a future you) picks up the thread. Collaboration happens the normal GitHub way: **issues** for open questions and hand-offs, **pull requests** for contributions. Anyone joining your mission just contributes to your repo; the git history is the honest record of who did what.

## 5. Prove
Before you call anything a finding, run the gate: **discover** the pattern on one slice of the data, **freeze** it (the exact relationship, thresholds, coefficients), and **confirm** it on a slice you never touched while searching. If it does not replicate there, it was a ghost, and you log that too. An independent dataset that never went into the search (a reanalysis, a held-out year, a separate instrument) is the cleanest confirmer.

## 6. Surface
Write it up honestly in your repo's `README.md` and `results/RESULTS.md`, then add your chip to the roster: edit `roster.json` in this repo via a pull request. The chip has a status:

| status | chip | meaning |
|---|---|---|
| `scout` | amber | claimed, just starting |
| `build` | teal | actively working, results coming |
| `found` | pink | a finding that cleared the one rule (step 5) |

Set the `link` to **your work** (a per-mission repo, or the dive's folder in your dives repo, e.g. `https://github.com/royber34/hiddentide-dives/tree/main/01-lighthouse-diary`) so the flag points at the real thing. Close your claim issue, referencing the merge.

## Honesty rules (non-negotiable)
- **Nulls are results.** "We looked, it was not there" is worth logging and is not a failure.
- **Cite every source and number.** Link the archive; a claim without a traceable source does not go in.
- **Do not overclaim.** State what you can defend and no more; write the caveats in the same breath as the result.
- **Confirm before you believe it.** The one rule, above, is the whole discipline.

That is the entire process. Pick, claim, dive, log, prove, surface. Welcome aboard.
