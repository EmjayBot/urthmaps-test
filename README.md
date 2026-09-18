# urthmaps-test

Test bed for automatic map layer sync into
[urth-atlas](https://github.com/EmjayBot/urth-atlas).

- Source of truth: `maps/source/urth.xcf` (GIMP 3)
- Push an XCF change → `.github/workflows/xcf-sync.yaml` exports the five
  mapped layers headlessly and commits PNGs to `atlas/` + `assets/`
- urth-atlas pulls `atlas/*.png` via its `map-imagery.yml` workflow

Tooling lives in [xcf-git-sync](https://github.com/EmjayBot/xcf-git-sync).
