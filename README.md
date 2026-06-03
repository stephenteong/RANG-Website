# RANG — Agency Website

Creator-led social media agency website. Built in HTML/CSS with embedded SVG logos, scroll-reveal animations, and three campaign video integrations.

---

## File Structure

```
rang-website/
├── index.html              ← Main website file (Campaign grid + editorial reasons)
├── v_asus.mp4              ← ASUS Black Friday campaign (1280×720, ~5.6MB)
├── v_msft.mp4              ← Microsoft Co-Pilot campaign (720×1280, ~4.0MB)
└── v_xbox.mp4              ← ASUS × Xbox campaign (720×1280, ~4.1MB)
```

---

## Previewing Locally

Videos only autoplay when served over HTTP — opening an HTML file directly from your desktop (`file://`) will block them.

**Option A — Run a local server**
```bash
# Python (no install needed on Mac/Linux)
cd rang-website
python3 -m http.server 8080
# then open http://localhost:8080
```

**Option B — VS Code**
Install the Live Server extension, right-click `index.html`, and choose "Open with Live Server."

---

## Sections

1. **Hero** — Full-viewport split: RANG wordmark + tagline left, ASUS campaign video right with 12M+ stat overlay
2. **As Seen In** — HYPEBEAST, VICE, CBC, Toronto Star
3. **Clients** — ASUS, Microsoft, ByteDance, Xbox
4. **About** — Reangsei Phos founding story and agency methodology
5. **Why RANG Delivers Results** — 5 reasons across three layout variants
6. **Campaigns** — ASUS Black Friday, Microsoft Co-Pilot, ASUS × Xbox with stats and campaign descriptions
7. **Services** — Social Media Management, Video Production, Brand Strategy, Influencer Marketing
8. **Contact** — hello@rang.agency

---

## Tech Notes

- **No frameworks or dependencies** — pure HTML and CSS, one Google Fonts import
- **Fonts** — DM Sans (300/400/500) + DM Mono (300/400) via Google Fonts
- **Logos** — Inline SVG symbols in `<defs>`; ByteDance uses real path data decoded from bytedance.com
- **Videos** — H.264, faststart flag for instant playback, no audio track
- **Animations** — IntersectionObserver scroll reveals, no library required
- **Campaign hover** — Hovering one video fades and pauses the others via vanilla JS
- **Mobile** — Responsive breakpoints at 960px and 680px

---

## Pending Items

Before final launch, the following still need to come from Reangsei:

- [ ] Permanent brand colour (cobalt blue is placeholder; currently black/cream only)
- [ ] Xbox campaign metrics (currently showing TBC)
- [ ] Reangsei's personal one-liner for the About section (optional)
- [ ] Custom domain setup
- [ ] Client testimonials (optional future section)

---

## Contact

**Agency:** RANG  
**Email:** hello@rang.agency  
**Website:** rang.agency  
**Founder:** Reangsei Phos — reangsei@rang.agency
