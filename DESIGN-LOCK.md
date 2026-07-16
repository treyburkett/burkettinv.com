# Burkett Domain Design Lock

SSOT for burkettinv.com, Perspectives, OS (app), Work (ops), Deals (tools).
**Out of scope:** The Panel.

Approved reference DNA: Tesla Cybertruck Specs page + Cursor dark UI + the wordless **cyber switch** on the main nav.

## Geometry
- `border-radius: 0` everywhere on chrome and marketing
- 1px hairlines only (no soft shadows, no pills, no cards-as-decoration)
- Sharp rectangular controls; cyber switch = track + sliding square knob

## Color
| Token | Hex | Use |
|-------|-----|-----|
| Black | `#000000` | Canvas, nav, chrome |
| Steel | `#141414` / `#1c1c1c` | Elevated panels |
| Line | `#2a2a2a` / `rgba(255,255,255,0.12)` | Hairlines |
| White | `#ffffff` | Primary values / headings on dark |
| Mute | `#8a8a8a` | Labels ABOVE values |
| Gold | `#ead4a2` | Brand ignition / CTA / active / switch hover |
| Gold deep | `#b6a57e` | Hover fill, light-mode logo accent |
| Burkett red | `#e31937` | Semantic only: risk, alert, negative, destroy |
| Burkett blue | `#3e6ae1` | Semantic only: info, link, focus, data highlight |

Gold remains the only marketing ignition. Red and blue never replace gold on CTAs or nav chrome. Drop legacy Burkett `#c9a23c`. Logo PNG/SVG files stay byte-identical.

## Type
- `system-ui` only (no Cormorant, Jost, Playfair)
- Specs pattern: **small grey label above large white value**
- Uppercase micro-labels: ~11px, tracking ~0.12–0.16em
- Headings: weight 600, tight tracking (-0.02 to -0.03em)

## Layout (marketing)
- Nav: always black; reverse logo; uppercase links; primary CTA; cyber theme switch (no words)
- Hero: one full-bleed apartment photo, copy bottom-left, dark scrim
- Performance row: 4 label/value cells, hairline dividers
- Dimensions block: left specs grid, right one large photo in hairline frame (no captions)
- Services / approach: hairline grids and numbered rows, not photo-stuffed cards
- Few photos (hero + one dimensions plate). No captioned strips.

## Theme
- Default dark
- Light mode: white page canvas, black type; **nav stays black**
- Toggle = cyber switch only

## Product chrome (OS / Work / Deals)
- Same tokens; true black runner; gold hairline; radius 0
- Controls inherit cyber sharpness (no rounded pills)

## Copy
- No Nashville HQ marketing on public surfaces
- Gulch board credential in bio OK
- Public voice is consulting + investment management expertise (see VOICE.md). Do not claim firm ownership of a portfolio until true.
- Type on this Next rebuild uses Geist + Geist Mono (self-hosted). DESIGN-LOCK `system-ui` still applies to legacy HTML / product chrome until those migrate.
