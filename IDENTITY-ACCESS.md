# Identity guidelines: Cloudflare Access

Public marketing stays open. Brand guidelines live at `/identity/` and must not be public.

## Why `/identity/` (not `/brand/`)

`/brand/*` holds public lockups and favicons used by the live site and email signatures. Access on `/brand*` would break those assets. Guidelines only: `/identity*`.

## Dashboard setup (one-time)

1. Cloudflare Zero Trust -> Access -> Applications -> Add an application -> Self-hosted.
2. Name: `Burkett Identity`
3. Application domain: `burkettinv.com`
4. Path: `/identity*` (include subpaths)
5. Policy: Allow emails ending in `@burkettinv.com` (or Kyle + Trey only). Use the same IdP as Ops (Entra / Microsoft).
6. Session duration: match Ops Board (e.g. 24h).
7. Do **not** put TAKE-DOWN deny-all on this app. Staff should be able to open it while OS/Work/Deals stay denied.

## After Access is live

Bookmark: `https://burkettinv.com/identity/`

Public nav and sitemap intentionally omit Identity. Wordmarks stay at `/brand/*.svg`.
