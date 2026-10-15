# CanYouSpeakEnglish external data

Trial data for a VRChat word explanation game. 64 selected noun senses: 16 each for CEFR-J A1, A2, B1 and B2. The full dictionary and unreviewed candidates are not hosted here.

- Catalog: v1/catalog.json
- Packs: v1/{A1,A2,B1,B2}/{000..031}.json
- Each pack contains at most 64 items; unused slots contain an empty items array.
- Item columns: id, en, ja, level, pos, synset, hintEn, hintJa.
- Require matching schema and revision between catalog and pack. Never treat an empty or failed download as a valid question.
- Existing v1 paths remain fixed for VRChat baked VRCUrl arrays. Breaking changes use a new schema path.
- Each item ID binds CEFR-J 1.6 row and WordNet synset. Review meanings before extending the trial.

See [CREDITS](CREDITS.md) for sources, modifications and licenses.
