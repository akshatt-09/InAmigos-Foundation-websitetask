# InAmigos Foundation — NGO Awareness Website

A single, dependency-free HTML/CSS/JS webpage built for Internship Task 1. Open `index.html`
directly in any browser — no build step, no framework, no server required.

## Files

```
inamigos-ngo-awareness/
├── index.html      # all page content and structure
├── style.css        # design system + layout + responsive rules
├── script.js         # nav scroll state, mobile menu, scroll-reveal, number count-up
├── README.md
└── assets/images/    # drop-in folder for real photography (see below)
```

## Content & accuracy

All facts, figures and initiative descriptions (Bachpanshala, Udaan, Jeev, Seva, Prakriti,
Vikas; the 50,000+ / 28 / 200+ / 6 statistics; founding date; certifications; events; contact
details) were taken directly from the official InAmigos Foundation website
(inamigosfoundation.org.in — home, About Us and Events pages) on the date this project was
built. Nothing was invented; where a detail (e.g. state-level project locations, non-verified
social links) wasn't published officially, the site uses neutral wording instead of guessing.

## Images

Real official photography could not be downloaded into this environment, so every image slot
uses a clearly labelled, styled placeholder (`.img-placeholder`) instead of a broken `<img>` tag
or an uncredited stock photo. To finish the project for submission:

1. Save real, permitted images into `assets/images/` using these names: `hero.jpg`,
   `bachpanshala.jpg`, `udaan.jpg`, `jeev.jpg`, `seva.jpg`, `prakriti.jpg`, `vikas.jpg`,
   `gallery-1.jpg` … `gallery-6.jpg`.
2. Swap each `<div class="img-placeholder">…</div>` for an `<img src="assets/images/…" alt="…">`
   with `loading="lazy"` and `style="object-fit:cover"` (classes already provide sizing).
3. The official gallery is linked at the bottom of the Gallery section for reference:
   https://inamigosfoundation.org.in/gallery

## Features

- CSS-only "Choose Your Cause" tab interaction (radio inputs, no JS)
- Sticky navbar with blur-on-scroll, mobile hamburger menu
- Scroll-reveal fade-ups and animated stat counters (IntersectionObserver)
- Respects `prefers-reduced-motion`
- Fully responsive (desktop / tablet / mobile), semantic HTML, visible focus states, alt text
  placeholders ready for real images
