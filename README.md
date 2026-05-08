# gef-render-assets-public

ACAP commercial render input assets.

PNG and JPG files used as input to the ACAP rendering pipeline
(`/v1/composite` on gef-acap-compositing). Hosted publicly so Railway
runtime can fetch them via raw URLs.

These are NOT:
- deterministic infrastructure fixtures (those live in `acap-fixtures`)
- commercial golden baselines (those live in a private baselines repo)
- final rendered outputs (those are local Francesca-review artifacts)

These ARE: input materials (foreground + background) for the renderer.

Each file is referenced by URL + sha256 in a manifest_ref.

## Files (FASE 2 — validation)

- `icepack-bg-warmgrey-2048.png` — 2048×2048 deterministic warm-grey gradient background
- `icepack-fg.png` — 500×506 RGBA Sogeva ICE plastica (busta + cartone), white-to-alpha cutout deterministic
