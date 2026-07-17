# Path to all As (Identity panel)

Target grades after this program (all A or A- with published gates):

| Persona | Now | Target | Unlock |
|---------|-----|--------|--------|
| Design Systems | B+ | A | Product control floor + OsShell SSOT + governance |
| Brand Strategy | A- | A | Shippable partner/deck artifacts (not rules only) |
| Apple Platforms | B+ | A | Live frosted-steel chrome demo + OK/NOT OK + Surfaces sync |
| Product Eng | C | A | Shared shell + focus sync OS + forms/tables |
| Motion / Film | C+ | A | CSS duration tokens + 6s beat sheet + 12-20s loop + ban CI |
| Accessibility | B | A | Exact dark+light ratios + enforcement beyond Identity |

Out of scope for all-A: Storybook app, full Polaris catalog, multi-cut film production, Access/ops setup.

---

## What "all As" looks like (one picture)

A builder (human or agent) can:

1. Open `/identity/` + `DESIGN-LOCK.md` + `globals.css` + `os-shell.css` and invent **zero** colors, radii, or focus rules.
2. Ship a form + table that matches Command Center density.
3. Hand a partner a one-pager + deck that cannot invent holdings claims.
4. See frosted steel only as chrome (never nested glass).
5. Use motion tokens from CSS; silent cutdown has a beat sheet; hero loop respects reduced-motion.
6. Pass dark + light contrast checks with published measured ratios; CI fails on drift.

---

## Parallel workstreams (multi-agent)

Run **Wave A** tracks in parallel (4 makers + 1 shared checker). Then **Wave B** (2 makers + OS sync). Then **Wave C** (reconvene panel + deploy).

```
Wave A (parallel)
  Track 1 Brand pack --------+
  Track 2 Apple Extend visual +
  Track 3 Motion tokens/loop +---> Wave A checker
  Track 4 A11y exact ratios --+

Wave B (parallel, after A or overlapping where safe)
  Track 5 Controls floor (forms/tables) ----+
  Track 6 OsShell SSOT + OS focus blue sync +---> Wave B checker
  Track 7 Governance strip + hub ------------- +

Wave C
  Panel reconvene (6 advisors) -> all A/A- or punchlist
  Deploy burkettinv.com + owner-portal if OS CSS changed
```

### Track ownership (Grok makers)

| Track | Maker focus | Artifacts | Depends |
|-------|-------------|-----------|---------|
| 1 Brand | Apply + VOICE + Drive templates | Partner one-pager HTML/PDF, deck skeleton, disclaimer copy-chip SSOT, co-brand card, proof lexicon export | none |
| 2 Apple | Extend + Surfaces | Photo-under-frost chrome demo, OK/NOT OK pair, glossary line, Reduce Transparency static pair | none |
| 3 Motion | globals.css + Foundations + Apply | `--duration-*` vars, 6s beat sheet, 12-20s silent hero loop (reduced-motion safe), ban grep list | none |
| 4 A11y | Controls + DESIGN-LOCK | Exact ratio table dark+light, light theme strip, dim lint note | none |
| 5 Controls | identity-controls + ui primitives | Field, select, checkbox, table, toast/alert with states | Track 4 focus/a11y law |
| 6 Product/OS | Surfaces + owner-portal os-shell.css | OsShell real specs, focus blue in OS, token bridge note, coding entry checklist | Track 5 demos for parity |
| 7 Governance | Hub + DESIGN-LOCK | Version/changelog strip, "agents must not invent" | after A |

### Objective gates (auto)

**Wave A**
1. Disclaimer string identical in VOICE.md + Apply copy-chip
2. Extend shows chrome-only frost over photo + NOT OK nested glass; no Vine
3. `globals.css` has `--duration-micro|control|panel|reveal`; Foundations cites them
4. Apply has filled 6s beat sheet + live or CSS hero loop with PRM kill
5. Controls a11y table uses exact ratios (no "~") for dark AND light

**Wave B**
6. Controls documents field + table + alert with focus/disabled/error
7. `os-shell.css` `:focus-visible` uses blue (or shared token), not gold
8. Surfaces OsShell is SSOT specs (or deep-link to CSS) not "marketing only"
9. Hub shows version + last-changed + invent bans
10. `npx next build --webpack` exit 0; portal pages still 200

**Wave C**
11. Six advisors regrade; each A or A- with cited gate
12. Deploy Identity (+ portal if OS CSS changed)

### Checker personas (separate from makers)

- Design Systems checker: token parity spot-check 12 tokens
- Brand checker: cold partner test (deck + one-pager, no Identity browse)
- Product checker: form+table built from Identity only invents nothing
- A11y checker: ratio script or manual luminance board; OS focus not gold
- Apple checker: visual chrome-only + grep Liquid Glass misuse
- Motion checker: duration vars present; beat sheet filled; ban list greppable

### Loop

- Manifest: `loop-manifest-identity-path-to-a.json`
- Pattern: build-audit-fix
- max_cycles: 5 per wave (design)
- Model: `cursor-grok-4.5-high-fast` makers/checkers
- Cap: stop when Wave C panel all >= A-

### Suggested calendar (2-person firm)

| Day | Parallel |
|-----|----------|
| 1 | Tracks 1-4 Wave A |
| 1 end | Wave A checker |
| 2 | Tracks 5-7 Wave B (OS focus sync + Controls floor) |
| 2 end | Wave B checker |
| 3 | Panel reconvene + deploy |

### Explicit non-goals

- Storybook
- Full modal/datepicker/chart catalog
- Real Apple native app
- Multi-cut brand film with audio
- Migrating all legacy HTML off system-ui in this program

---

## Decision for Trey

Approve Wave A start (tracks 1-4 parallel). Wave B touches live OS CSS (focus blue); confirm before that track runs.
