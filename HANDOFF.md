# burkettinv.com rebuild (Cybertruck / Cursor)

Founder-led consulting and investment management. Cybertruck spec-sheet UI +
Cursor dark-tool aesthetic. Public voice: expertise sold across asset classes,
not a claim of owned holdings. See `VOICE.md` and `DESIGN-LOCK.md`.

## Stack
- Next.js 16 (App Router) + React 19 + TypeScript
- Tailwind CSS v4 (tokens in `app/globals.css`)
- Geist + Geist Mono (self-hosted via the `geist` package)
- motion, @phosphor-icons/react
- Static export (`output: "export"`) for Cloudflare Pages / GitHub Pages

## Pages
- `/` home, `/platform`, `/expertise` (legacy `/portfolio` redirects),
  `/perspectives` (+ one article), `/about` (Firm), `/contact`.
- `/identity/` brand guidelines (internal; not in public nav). Protect with Cloudflare Access (`IDENTITY-ACCESS.md`). Public lockups stay under `/brand/*.svg`.
- Login / Owner Login restored in nav + footer → `SITE.loginUrl` (app.burkettinv.com).

## Run it
```
npm install
npm run dev          # http://localhost:3000
```

## Build the deployable site
```
npx next build --webpack
```
Deploy the contents of `out/` to the live `burkettinv.com` static host.
Preserve `the-panel/`, `qb-callback/`, `CNAME`, favicons, robots, sitemap.

## Products
OS / Work / Deals stay Access-denied until Login copy matches private/building truth.
See `TAKE-DOWN.md`.

## Cloud Agents (later)
This Next source lives at `~/Developer/burkett/burkettinv-next` and is not yet its own GitHub repo. When you want phone-driven copy PRs: `git init`, push to a GitHub remote, connect it in Cursor Cloud Agents, set a spend cap. Hosting stays the static `out/` deploy to `burkettinv.com` (GitHub Pages / Cloudflare).
