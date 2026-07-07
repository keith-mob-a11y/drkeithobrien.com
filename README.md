# drkeithobrien.com

Static one-page site for Dr Keith O'Brien's executive coaching practice. Hand-written HTML/CSS/JS, zero build step, zero runtime dependencies, no external requests (fonts self-hosted).

## Deploying

Push to `main`. GitHub Pages serves the repo root. That's it.

## Common edits

| Change | Where |
|---|---|
| Booking link | Search `calendar.app.google` in `index.html` (4 occurrences: nav, hero, final CTA ×2) |
| **Add a real testimonial** | `index.html` → uncomment the `TESTIMONIALS` section; copy the `<figure class="quote-card">` block per quote. **Never publish placeholder/invented quotes** |
| Fees | `index.html` → `#fees` section. Keep in sync with the vault Rate_Card |
| Foundation places count | The `fees-foundation` paragraph; update or remove when the four places are gone |
| ACC awarded | Swap 'completing the Professional Certificate…' / 'completing my ICF accreditation' wording in About + FAQ; consider adding the ACC badge to `.badges` and the credentials strip |
| Lead magnet PDF | Replace `assets/first-90-days-with-ai.pdf` (keep the filename, or update the link in `#guide`) |
| New article/insight pages | Create `insights/slug/index.html` reusing the head + nav + footer; add to `sitemap.xml`. Pattern intended for repurposing LinkedIn pillar content |
| Analytics | Uncomment the Cloudflare beacon in `<head>`, add token |
| OG image | Regenerate from the og.html template (Dex has it) → `assets/og-image.png`, 1200×630 |

## Design tokens

All in `:root` in `styles.css` — ivory `#F7F3EA`, ink `#17293D`, brass `#9A6B21`. Display font: Fraunces (self-hosted variable woff2, weights 300–700). Body: native humanist sans stack.

## Rules of the house

British English. No em-dashes. No fake testimonials, no fake scarcity, no popups, no email gates, no cookie banners (nothing here needs consent). Page weight budget: ≤ 350KB excluding photos.
