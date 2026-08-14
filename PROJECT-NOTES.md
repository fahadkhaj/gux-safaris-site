# GUX Safaris — Site Update Notes

## What changed in this round

**Logos** — reorganized into `assets/images/logo/` with clear names:
- `gux-logo-horizontal-light.png` — used in header nav & footer (both sit on dark backgrounds)
- `gux-logo-horizontal-dark.png` — used anywhere the logo sits on a light/white card
- `gux-icon-mark.png` — favicon
- `gux-og-share.png` — social share preview image (Facebook/WhatsApp/Twitter link previews)
- `gux-logo-stacked-light/dark.png`, `gux-logo-mono-black/white.png`, `gux-social-badge.png` — kept for future use (business cards, social avatars, merch, etc.), not currently wired into the site

**Colors** — pulled the real palette straight from your logo files instead of guessing:
- Deep brown `#2E1B10`, rust `#84482A`, warm terracotta `#C17A45`, espresso `#3D2314`, cream `#FAF0D9`
- Applied everywhere via the `--brand-*` CSS variables already used across the pages

**Fonts** — wired in the Jura font you had bundled in `assets/fonts/`, now used for all headings site-wide.

**New pages:**
- `destinations.html` — full categorized guide (Northern Circuit, Southern & Western Parks, Zanzibar, Trekking & Adventure) covering everything on your list. Places with an existing detail page link there; the rest link to the contact page for now since there's no dedicated page yet.
- `our-story.html` — the GUX Safaris brand story page.
Both are linked from every page's nav, mobile menu, and footer.

**Bugs fixed:**
- Ruaha's three broken thumbnail images (were pointing at a folder that doesn't exist)
- The booking popup's dropdown had 8 options all wrongly set to `"zanzibar"` — now each option has its own correct value
- A dead "News & Updates" link (no news page exists) was removed from nav/footer everywhere
- Index page's "Home" link pointed to `#` instead of `index.html`
- All booking/contact forms now show a "we'll be in touch" confirmation instead of silently failing, since there's no backend yet — swap this out once you have one

## Still needs your input
- **Zanzibar & several southern parks** (Saadani, Katavi, Rubondo, Saanane, Mahale Mountains, Mkomazi, Mount Meru, Usambara, etc.) don't have real photos in your assets folder yet, so their cards on the destinations page use a styled placeholder instead of a photo. Send real images when you have them and I'll drop them in.
- Facebook/Instagram links are still placeholders (`facebook.com/guxsafaris`, `instagram.com/guxsafaris`) — swap for your real handles.
- Contact email is `info@guxsafaris.com` as a placeholder per your earlier note.
