# Anvaya English

**Anvaya** — अन्वय, the joining of words into meaning.

Anvaya English dissects the understanding and the underlying thought of a text — who does what to whom, what rests on what — and hands that map to an agent, so the agent can grasp the writing quickly, from measured structure instead of from fog.

## What it is

Anvaya English is the English language edition of the Codetopo family. It turns a passage of English into a graph an agent can query: the sentences, the predicates (the actions), and the noun-phrase entities (the things), joined by the relations between them.

The graph has two storeys, and the two are never blurred:

- **The grammar floor** — grammatical relations (subject-of, object-of, modifier-of, and the rest) extracted by a real, pinned parser: spaCy 3.8.18 with the en_core_web_md 3.8.0 model. Every one of these edges is stamped **inference**: a parser's reading is a measurement with an error rate, and the graph says so.
- **The claims floor** — the connections across sentences (what a pronoun points back to, which sentence carries the main claim, what supports it). These cannot be extracted by rule. They are added by a reading agent and stored as **declared claims**, each one naming its claimant and its written basis.

Every Anvaya English graph is **claims-class**. It never presents itself as truth-class, and no edge ever loses its label.

## Measured accuracy

On the fixture paragraph (the opening of Codetopo's own DESIGN.md, seven dense sentences), with every grammatical relation checked by eye against the text:

- **119 of 137 relations correct — 86.9%.**
- A plain sentence is near-flawless; the thesis sentence scored 100%.
- The errors gather in three named places: parentheticals and hyphenated names; lists after colons; chained coordination.

The full audit — every flaw named, per-sentence scores — is the product's published accuracy statement, kept with the engine: [docs/english-accuracy.md](https://github.com/nrupala/codetopo/blob/main/docs/english-accuracy.md). A change that moves a count moves that statement in the same change.

## In this repo

- `profile/english.profile.json` — the edition's engine profile, copied byte-for-byte from nrupala/codetopo.
- `companion/` — the ingest companion: grammar edges only, and it refuses any parser but the pinned one.
- `docs/` — the product documentation: the profile doc and the published accuracy statement.
- `fixture/` — the known-answer fixture: the paragraph, the two-storey snapshot, and the derivation notes.
- `PROVENANCE.md` — the source commit, the file map, and the hash proof for every copied file.

## State

- The engine profile is **built and merged** in [nrupala/codetopo](https://github.com/nrupala/codetopo) — PR #171, merge commit `3158760b`. The profile, the ingest companion (which emits grammar edges only, and refuses any parser but the pinned one), the fixture, and the accuracy statement all live there today.
- This repo is the product's own home: packaging, product documentation, and releases gather here.
- **Release gate: NOT RUN. Guardian Mesh: NOT RUN.** Anvaya English is not yet a certified release. Nothing here is a sales claim, and no price is set for Anvaya — pricing is the Director's, and none has been set.

## Licence

AGPL-3.0. © 2026 2351485 ALBERTA INC. / AIMLDS.
