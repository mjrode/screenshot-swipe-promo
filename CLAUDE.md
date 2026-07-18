# promo-page — screenshotswipe.com

Marketing site + blog for **Screenshot Swipe: Smart Notes** (iOS, App Store id
6757885971; app source in `../screenshot-swipe`). This is the REAL site — the
sibling repo `../screenshot-swipe-privacy` (mjrode.github.io) is privacy-policy
hosting only and redirects here.

## Layout

Plain static HTML — no framework, no build step.

| Path | Purpose |
|---|---|
| `index.html` + `styles.css` | Promo landing page (scroll-animation design — its own stylesheet) |
| `blog/index.html` | Blog index — cards maintained manually between `BLOG_GRID` markers |
| `blog/[slug]/index.html` | Posts (self-contained; copy an existing post as scaffold) |
| `blog/[slug]/assets/` | Post images (WebP only) |
| `blog.css` | Blog + privacy stylesheet (separate from the landing's `styles.css`) |
| `assets/blog/` | Shared blog assets: app icon, favicon, marketing shots (`shot-*.webp`) |
| `privacy/index.html` | Canonical privacy policy |
| `scripts/make-cover.py` | Deterministic Pillow blog-cover compositor |
| `seo-tools/` | `product-context.md` (product facts) + `TODO_SEO.md` (keyword backlog) |
| `.agent/skills/` | Content skills (symlinked into `.claude/skills/`) |

## Deployment

GitHub Pages (repo `mjrode/screenshot-swipe-promo`, `main` branch root) with
CNAME `screenshotswipe.com`, fronted by Cloudflare. **Push to `main` = deploy.**
Cloudflare caches HTML for ~10 min — hard-refresh or purge cache when verifying.

Internal links are root-absolute (`/blog/...`); canonical/og URLs use
`https://screenshotswipe.com/...`.

## Writing blog posts

Use the `blog-post-generator` skill (`.claude/skills/blog-post-generator/SKILL.md`) —
it carries the editorial voice rules (shared with GainFrame), the JSON-LD entity
contract, and the publish checklist (post + index card + sitemap entry in one commit).

## Constraints

- Never touch `styles.css` for blog work — blog pages use `blog.css`.
- Never remove `/privacy/`.
- Author entity is always Michael Rode with `url: https://gainframe.app/about`.
