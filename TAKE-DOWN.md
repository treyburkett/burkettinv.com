# Product take-down (2026-07-10)

Reversible. Nothing deleted.

## What changed

1. Marketing (burkettinv.com): Login and Owner Login removed from the public site (Next rebuild cutover). Do not re-add until product copy matches private / building truth.
2. Cloudflare Access: Policy `TAKE-DOWN deny all` (deny everyone, precedence 1) on:
   - app.burkettinv.com
   - ops.burkettinv.com
   - tools.burkettinv.com
   - ops-api.burkettinv.com
   - cc-api.burkettinv.com
   - burkett-portal.pages.dev
   - *.burkett-portal.pages.dev
   Existing allow policies kept at precedence 10+.

## Restore

1. Re-add Login / Owner Login in the Next source (`burkettinv-next` nav/footer), rebuild `out/`, deploy, commit, push.
2. Cloudflare Zero Trust -> Access -> each app -> delete policy named TAKE-DOWN deny all (or set allow policies back to precedence 1).
3. Optional API: DELETE `/accounts/{id}/access/apps/{app_id}/policies/{policy_id}` for each deny policy named `TAKE-DOWN deny all`.

## Source of truth

Live static site is built from `~/Developer/burkett/burkettinv-next` (`npx next build --webpack` → `out/`). Voice: `VOICE.md`. Design: `DESIGN-LOCK.md`.
