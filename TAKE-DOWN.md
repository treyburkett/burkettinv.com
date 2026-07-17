# Product take-down (2026-07-10) — restored 2026-07-16

## Restored

1. Marketing: Nav **Login** + footer **Owner Login** → `https://app.burkettinv.com` (deployed `c080b14`).
2. Cloudflare Access: deleted `TAKE-DOWN deny all` on app, ops, tools, ops-api, cc-api. Owner allow policies remain.
3. Portal deploy to `burkett-portal` is live.

## Identity guidelines

Brand guidelines are at `/identity/` (not in public nav). Protect with Cloudflare Access path `/identity*` so public `/brand/*.svg` lockups stay open. Steps: `IDENTITY-ACCESS.md`.
