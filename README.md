# VELORIS DialLab

Engineering-first dial geometry tooling for VELORIS.

Current active gate: **P1 Geometry Core**. See `governance/CURRENT_GATE.md`.

The current implementation deliberately does **not** encode manufacturer-specific dimensions or tolerances. Geometry values are explicit inputs in millimetres. The SVG exporter preserves a 1:1 millimetre coordinate system and deterministic output so later engineering evidence can be reproduced and audited.

## Verify locally

```sh
npm run verify
```

`typecheck` uses TypeScript in `checkJs` mode; no emitted JavaScript is required. The build step copies the authoritative geometry module to `dist/` and writes a SHA-256 manifest.
