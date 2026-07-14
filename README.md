# Ross Katzenberg — Artist Portfolio

Immersive, hypnotic single-page portfolio. Full-bleed slowly-rotating mandalas,
responsive across mobile, tablet, and desktop. Static HTML/CSS — no build step.

## Structure

```
.
├── index.html          # the whole page
├── css/
│   └── style.css       # all styles + responsive breakpoints
└── images/
    ├── art-04.jpeg     # hero mandala (rotating)
    ├── art-08.jpeg     # quote-band mandala (rotating)
    ├── art-10.jpeg     # "The Buzzing Sound of Emptiness"
    ├── art-03.jpeg     # "Witness"
    ├── art-09.jpeg     # "The Screen"
    └── art-01.jpeg     # about-section emblem (rotating)
```

## Deploy to GitHub Pages

1. Create a repository (e.g. `ross-katzenberg-portfolio`) and push these files to the
   root of the `main` branch.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**,
   pick branch **main** and folder **/ (root)**, then **Save**.
4. Your site goes live at `https://<username>.github.io/<repository>/` within a minute.

### Custom domain (optional)
Add a `CNAME` file at the root containing your domain (e.g. `rosskatzenberg.com`)
and point the domain's DNS at GitHub Pages.

## Editing

- **Text / links** — edit directly in `index.html`.
- **Images** — replace files in `images/` (keep the same names) or update the
  `src` paths. Square-ish images work best for the rotating mandalas.
- **Motion** — spin speeds live in `css/style.css` (`.spin` / `.spin-r`,
  the `120s` / `150s` values). Motion auto-pauses for visitors who have
  "reduce motion" enabled in their OS.

## Responsive breakpoints

- Desktop: full 3-column works grid, side-by-side about section.
- Tablet (≤ 900px): about section stacks and centers.
- Mobile (≤ 620px): hamburger menu, single-column works, stacked contact.
