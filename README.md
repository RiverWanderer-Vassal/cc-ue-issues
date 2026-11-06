# Commands & Colors UE modules: bug reports

This is where to report problems with the **Ultimate Edition (UE)** VASSAL modules for GMT Games' Commands & Colors
series:

- Commands & Colors: Napoleonics UE
- Commands & Colors: Ancients UE
- Commands & Colors: Medieval UE
- Commands & Colors: Samurai Battles UE

**[Report a problem](../../issues/new/choose)**: pick your module's form. If the module itself hits an error, its
**Report** button opens the right form with the details filled in. Please attach the game log the module names: it
replays the game exactly, which is usually all it takes to find the fault.

This repository holds issues only; the modules' code is kept elsewhere. The older (non-UE) modules have their own
repositories: [ccnapoleonics](https://github.com/RiverWanderer-Vassal/ccnapoleonics),
[ccnapoleonicsEpic](https://github.com/RiverWanderer-Vassal/ccnapoleonicsEpic) and
[congressofvienna](https://github.com/RiverWanderer-Vassal/congressofvienna).

## What happens to a report

1. **needs-triage**: new; the game log is replayed to reproduce it.
2. **confirmed**: reproduced. The fix is made in the module's code repository and the issue here is closed by
   that fix (or the issue is moved there, when the details are best kept with the code).
3. **vassal-engine**: the fault is in VASSAL itself, not the module. It is forwarded to
   [vassalengine/vassal](https://github.com/vassalengine/vassal/issues) with a minimal example, and linked here.
4. **not-a-bug** / **duplicate**: works as the rules say, or already reported (linked).

## Training the computer opponent
Playing against the computer with **Training mode** ticked, you can comment on its moves; **Send training report…** then opens the *Training report* form here with your comments filled in. These carry the label **training** and stay apart from bug reports: each comment is replayed in the exact position and becomes a test the computer must pass (**to-review** → **case-added** → **bot-fixed**; **disagree** when we think its move stands, **data-only** when there is nothing to fix). A training report holds no player names and no chat; sending one makes that game public training data.

Rules questions and requests use the *Rules question or request* form. Please quote the rule book, card or FAQ.

A report without the game files gets the **needs-files** label and a note asking for them; the label comes off by
itself once a file is attached.

## Forwarding a VASSAL fault
When triage shows the fault is in VASSAL itself, not the module:
1. Reproduce it in the smallest case possible, ideally without the UE module's custom code.
2. Open an issue at [vassalengine/vassal](https://github.com/vassalengine/vassal/issues) with the VASSAL version,
   operating system and Java version, the steps, and the minimal example (log or saved game).
3. Link it here, label this issue **vassal-engine**, and keep it open until VASSAL has a fix or a workaround.

<!-- >>> cc-ue-core workflow (synced by cc-ue-core tools/align-repo.sh) -->
## Workflow
Changes to this repository follow the UE git workflow in `RiverWanderer-Vassal/cc-ue-core` `docs/workflow.md` (a branch and pull request per change, squash-merged). This repository holds issues and forms only: no code.
<!-- <<< cc-ue-core workflow -->

---
Commands & Colors: Napoleonics, Ancients, Medieval and Samurai Battles are designed by Richard Borg and published by
GMT Games, LLC; game material © GMT Games, LLC, used under GMT's terms for electronic versions. The UE modules are
unofficial: not GMT products and not endorsed by GMT Games or Richard Borg. Modules © 2026 Mark Benson, all rights
reserved.
