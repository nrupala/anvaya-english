# Provenance — Anvaya English

This repo is the product home of Anvaya English. The engine lives in [nrupala/codetopo](https://github.com/nrupala/codetopo). The files listed below are the edition's own assets, copied byte-for-byte from that repo and versioned here. The copy was made on 2026-11-20 from codetopo main at commit `d7c7068f9b57e468f46120d5490d431f55ead709`.

Every copied file was proven byte-identical to its source: the git blob hash of each copy equals the source blob hash in codetopo, and the SHA-256 of each file is listed below. The full comparison log is kept in the house work record (Anvaya stand-up — STATUS, 2026-11-20).

## File map

| In this repo | Source in nrupala/codetopo | Source blob | SHA-256 |
|---|---|---|---|
| fixture/README.md | crates/codetopo-core/tests/fixture-english/README.md | `a9b543a151bdc9b0c4fe97c393644af44cc90886` | `52bc9030470abba403c4f252c4828cf976e7a0186c82a0f6705464dce4e488ff` |
| fixture/paragraph.md | crates/codetopo-core/tests/fixture-english/paragraph.md | `4cef12243dfd88021c09b498d43536616a0be744` | `14da0aacf7158637e1412de6fe729e15ba61ad0fd3d700a014876d3c8c91271e` |
| fixture/paragraph.snapshot.json | crates/codetopo-core/tests/fixture-english/paragraph.snapshot.json | `f2640e4550a125820f44266a0124cec66dbfff1b` | `f9545538b7e2c88ff3f46a031aaf7021a317b791cae5991d742f2d169d8c56e4` |
| docs/english-accuracy.md | docs/english-accuracy.md | `ad0138827422cab11bc65fe1c159339c58942529` | `e9a35cd58ca0e5db065b6c315c274918eaba6d73acac4f424de825deaade8a68` |
| docs/english-profile.md | docs/english-profile.md | `f2cfae95a8771860554d9e91689f9d5b6eb91472` | `f9d503fb7160375562be82ddb7c60309a828217e22cad561235a2a5f8d104010` |
| profile/english.profile.json | profiles/english.profile.json | `b403cc7542f2c1b58c51992e2981f44c35cedf75` | `50c39df9c774553c35762725aa6b19ce69dcaef145d28837d8206e6cd559998e` |
| companion/README.md | tools/english-ingest/README.md | `dafc97afb5aa721ea3cbd2b4e998c4461d01f4ea` | `513a1aeaa09f6d3dde0148ca0efe422f4faf6ae576c20bf75c142853fac68d8e` |
| companion/english_ingest.py | tools/english-ingest/english_ingest.py | `feac2da8fae821caed65f1ff94377f776f7371b5` | `ea83b45b8f4bf45cbe2c7dce94e8da7e0b534544e520ec26f26b516c38cefc22` |
| companion/requirements.txt | tools/english-ingest/requirements.txt | `349b94acbb89b32ef4e071c1cb48b44fac8a0d05` | `41057df4491ba4941214238346c3045f1b989afa66a636c709ae08d7a39a1977` |

## The standing arrangement

- The engine — the profile loader, the clustered rendering, the store, the query surface — is built and maintained in nrupala/codetopo. This repo holds the edition's own assets: the profile data, the ingest companion, the product documentation, the fixture, and this note.
- When the copies in the engine repo move, the copies here are refreshed from them, and this file is updated with the new source commit in the same change. If a count in the accuracy statement moves, the statement here moves in the same change.
- State lines, unchanged: **Release gate: NOT RUN. Guardian Mesh: NOT RUN.** Nothing here is for sale, and no price is set.
