# Identity style guide (what we built)

## Answer in one line
Before: brand book (logo, palette, type, signatures). After Wave 1–3: full UI style guide mini-site under `/identity/` with Foundations, Controls (buttons + color-on-color), Mark, Surfaces, Voice, Apply, and Extend (Liquid Glass / short-form / kiosk honesty).

## Routes (Access on `/identity*`)
| Path | Job |
|------|-----|
| `/identity/` | Hub: 6 principles + chapter index |
| `/identity/foundations/` | Tokens, type, geometry, theme |
| `/identity/controls/` | Buttons, cyber switch, OK / Not OK color stacking |
| `/identity/mark/` | Wordmarks, clearspace, favicon rules |
| `/identity/surfaces/` | Marketing + OS layout recipes |
| `/identity/voice/` | Expertise copy rules |
| `/identity/apply/` | Email, decks, social, density |
| `/identity/extend/` | Liquid Glass mapping, ~6s brand motion, low-priority display |

## Preview
```bash
cd ~/Developer/burkett/burkettinv-next && npm run dev
# open http://localhost:3000/identity/
```

## Deploy (when Trey approves)
Build `out/`, rsync to `burkettinv.com`, push. Access already covers subpaths.

## Agents
- Audit: [coverage gap](8a5cce41-5a35-4690-ba71-8f99a578c91d)
- Architecture: [IA advisor](792f7564-15e1-4fdf-80eb-e4985768277b)
- Makers: Wave 1 [build](768807bb-761d-452e-b353-7762a799df2b), Waves 2–3 [build](da1b58c1-7864-4451-9f1f-66bb329355ae)
- Checkers: [Wave 1](eae4f75b-3abc-447c-b3d3-ff90522988f4), [Wave 2–3](2fa2327f-e976-4b32-9ee0-c39a8c180db8)
