# MandateOverhaul

A Europa Universalis IV mod that adds content around the Chinese Mandate of
Heaven. Target version 1.37.5.0. Requires the Mandate of Heaven DLC.

Vanilla treats the Emperor of China as a single tag holding a single mechanic.
The intent here is to make the mandate something that is *contested* — claimed,
lost, split between rival courts, and defended against the people who actually
threatened it — rather than a status one country happens to hold.

## What it adds

**Claiming the mandate.** A decision to proclaim the Mandate of Heaven, gated to
the countries that could plausibly advance such a claim: East Asian cultures, the
Chinese warlord kingdoms, and steppe hordes — and only with a province in China.
In vanilla the equivalent conditions leave the decision visible to nearly every
country in the game, Austria included.

**The collapse of Ming.** An event chain and a disaster for a Ming that is losing
control, with modifiers for the collapse itself, plus a casus belli for the
succession that follows.

**Feudatories.** Decisions, events and modifiers for the semi-autonomous
feudatory rulers a weakened Chinese state had to tolerate.

**Dongning and the Zheng.** An event chain for the Zheng regime on Formosa,
which did not regard itself as an *ally* of the Ming so much as the continuation
of it — it kept the Yongli calendar long after the mainland was gone. The chain
lets that relationship be chosen rather than assumed, and deliberately does not
bind Formosa into the mainland's defensive wars.

**Manchu missions.** Edits to the Manchu mission events, including the maritime
network and the Jurchen path toward the mandate.

## Install

Copy this folder into

    Documents/Paradox Interactive/Europa Universalis IV/mod/

and create a sibling `MandateOverhaul.mod` next to it containing the same lines as
`descriptor.mod` plus an absolute path, forward slashes:

    path="C:/Users/<you>/Documents/Paradox Interactive/Europa Universalis IV/mod/MandateOverhaul"

EU4 ignores the launcher's load order and resolves conflicts by mod *name*, with
the earlier-sorting name winning. Events, decisions and most `common/`
subdirectories here concatenate with vanilla rather than replacing it.

## Conventions

Lines changed in a copied vanilla file carry an `@` in the trailing comment with
the previous value, so a text search for `@` lists everything this mod touches.
Script files are CP-1252 with LF endings and no BOM; localisation is UTF-8 with
BOM. Both matter — EU4 fails quietly on the wrong one.

Chinese translations for this mod's localisation keys live in a separate mod, so
the language can be switched without touching gameplay.

## Note

`common/cb_types/00_cb_types.txt` is Paradox Interactive's file, copied because
that directory overrides by filename rather than merging, with edits marked as
above. This is an unofficial personal mod, not affiliated with or endorsed by
Paradox Interactive.
