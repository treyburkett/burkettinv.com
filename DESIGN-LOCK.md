# Burkett Domain Design Lock

SSOT for burkettinv.com, Perspectives, OS (app), Work (ops), Deals (tools).
**Out of scope:** The Panel.

Approved reference DNA: Tesla Cybertruck Specs page + Cursor dark UI + the wordless **cyber switch** on the main nav.

Live CSS SSOT for the Next marketing rebuild: `app/globals.css`. Identity guide: `/identity/`.

## Geometry
- `border-radius: 0` everywhere on chrome and marketing
- 1px hairlines only (no soft shadows, no pills, no cards-as-decoration)
- Sharp rectangular controls; cyber switch = track + sliding square knob

## Color (dark default)

| Token | Hex (dark) | CSS var | Tailwind | Use |
|-------|------------|---------|----------|-----|
| Black / canvas | `#08080a` | `--bg` | `bg-bg` | Canvas, chrome ink on light |
| Black deep | `#0d0d10` | `--bg-2` | `bg-bg-2` | Alternate bands |
| Steel / panel | `#111114` | `--panel` | `bg-panel` | Elevated panels |
| Elevated | `#17171b` | `--elevated` | `bg-elevated` | Raised controls |
| Line | `rgba(255,255,255,0.10)` | `--line` | `border-line` | Hairlines |
| Line strong | `rgba(255,255,255,0.17)` | `--line-2` | `border-line-2` | Stronger edges |
| White / fg | `#f4f4f5` | `--fg` | `text-fg` | Primary values on dark |
| Mute | `#9b9ba4` | `--muted` | `text-muted` | Body support |
| Dim | `#6a6a73` | `--dim` | `text-dim` | Micro-labels only (large text / UI chrome; not body) |
| Gold | `#ead4a2` | `--gold` | `bg-gold` / `text-gold` | Brand ignition / CTA / active |
| Gold deep | `#b6a57e` | `--gold-deep` | `bg-gold-deep` | Hover fill, light-mode logo accent |
| Burkett red | `#e31937` | `--bk-red` | `text-bk-red` | Semantic: risk, alert, destroy |
| Burkett blue | `#3e6ae1` | `--bk-blue` | `text-bk-blue` | Semantic: info, link, **focus ring**, data |

Light theme remaps canvas/type and gold to `#8a7231` (see `globals.css`). Nav stays black.

Gold is the only marketing ignition. Red and blue never replace gold on CTAs or nav chrome. Drop legacy `#c9a23c`.

## Focus
- Focus ring: **Burkett blue** (`--bk-blue`), 2px solid, offset 2px
- Gold is ignition (CTA / active), not the focus outline
- `:focus-visible` only (never steal mouse click outlines)

## Type
- Next marketing / Identity: Geist + Geist Mono (self-hosted)
- Legacy HTML / older product chrome: `system-ui` until migrated
- Specs pattern: small grey label above large white value
- Uppercase micro-labels: ~11px, tracking ~0.12 to 0.16em
- Headings: weight 600, tight tracking (-0.02 to -0.03em)

## Motion
| Token | Value | Use |
|-------|-------|-----|
| Ease | `cubic-bezier(0.16, 1, 0.3, 1)` | Only material ease |
| Micro | 120 to 160ms | Focus tint, hairline |
| Control | 200ms | Button, switch, link |
| Panel | 250 to 300ms | Drawer, tab panel |
| Reveal | 500ms | Scroll enter |
| Line draw | 550ms | Gold accent line |

Enter: opacity + `translateY(12px)` + `scale(0.985)`. Press: `scale(0.98)`. Stagger: 30 to 80ms, max ~5 siblings.
`prefers-reduced-motion: reduce` snaps to end state; kill marquee / reveal / film loops.

**Ban:** springs, bounce, overshoot, scale-from-zero, glow pulse, soft Ken Burns, trend audio, emoji stickers, confetti, scroll-jacking, soft glass bloom.

Silent cutdown (~6s): one idea, architecture/material/UI only. Not "Vine." Optional 12 to 20s web hero loop is separate.

## Layout (marketing)
- Nav: always black (owned web chrome); reverse logo; uppercase links; primary CTA; cyber theme switch
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
- Dense form/table recipes live with the OS repo; Identity Surfaces notes are density guidance, not a second OS SSOT

## Copy
- No Nashville HQ marketing on public surfaces
- Gulch board credential in bio OK
- Public voice is consulting + investment management expertise (see VOICE.md). Do not claim firm ownership of a portfolio until true.
- Client work vs firm capital: we advise and underwrite for clients; we do not present client assets as Burkett holdings.
