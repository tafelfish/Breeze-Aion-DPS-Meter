# Pet catalog provenance

Collection IDs, canonical vehicle asset keys, English names and genera are
derived from the MIT-licensed catalog at:
https://github.com/SkeeveAN/Aion-DPS-Meter/blob/cf495eaf827f552bf8899ef06ef0fbb72f54ec05/Client/assets/aion2/pets/pets.json

The accompanying license is `licenses/pet-catalog-MIT.txt`. Game names belong
to NCSOFT. No tracker application binaries or implementation were imported.

Map associations use the existing community map data (see
`public/companion/maps/SOURCE.txt` and `licenses/companion-notices.txt`).
The generator compares the canonical vehicle portrait asset key, then requires
the same existing marker ID, subtype and exact coordinates. It never matches
translated or approximate pet names. Multiple locations are retained.

Generated with `tools/import-pets.py` on 2026-10-19. No map images are replaced.
Catalog inclusion does not guarantee availability in every region or patch.

Tracker portraits are bundled from https://resource-aion2.tc-imba.com/ using
the pinned catalog's exact vehicle asset key for each collection ID. The
resource path is `UI/Resource/Texture/Portrait/Portrait_Vehicle/` followed by
`UT_Vehicle_Portrait_{key}.webp`. `tools/import-pet-icons.py` validates the
image format and preserves the existing collection and map associations.
Game artwork belongs to NCSOFT; community resource attribution and the
noncommercial data license are recorded in `licenses/companion-notices.txt`.

The same pinned catalog supplies the exact NPC-template to collection mapping
in `src-tauri/src/pets/npc-pets.json`: 2,256 templates map to 192 of the 207
catalog pets. Unmapped templates are ignored. These mappings support recently
observed spawn notices; they do not establish a creature's distance or prove
that it remains present. No third-party tracker implementation was copied.
