# Product take-down (2026-07-10) — partially restored

## Restored (2026-07-16)

1. Marketing: Nav **Login** and footer **Owner Login** restored in Next source (`site-nav.tsx`, `site-footer.tsx`) → deploy via `out/` to burkettinv.com.
2. Portal deploy to `burkett-portal` is live again.

## Still blocked until Access deny is removed

Cloudflare Access policy `TAKE-DOWN deny all` (deny everyone, precedence 1) may still be on:

- app.burkettinv.com
- ops.burkettinv.com
- tools.burkettinv.com
- ops-api.burkettinv.com
- cc-api.burkettinv.com
- burkett-portal.pages.dev
- *.burkett-portal.pages.dev

## Finish restore

1. Cloudflare Zero Trust → Access → each app → delete policy named `TAKE-DOWN deny all` (or set allow policies back to precedence 1).
2. Optional API: DELETE `/accounts/{id}/access/apps/{app_id}/policies/{policy_id}` for each deny policy named `TAKE-DOWN deny all`.

## Identity guidelines

Brand guidelines are at `/identity/` (not in public nav). Protect with Cloudflare Access path `/identity*` so public `/brand/*.svg` lockups stay open. Steps: `IDENTITY-ACCESS.md`.
