# Barbershop Concept Previews

Unofficial, single-file concept preview websites built for local barbershops. Each is a self-contained `index.html` (no build step, no dependencies) styled around real details pulled from each shop's public listings, socials, and reviews.

These are **not affiliated with or published by** the businesses they're built for — they're design concepts, intended as a starting point a shop owner could hand to a developer or use as-is.

## Sites

| # | Shop | Location | Folder |
|---|------|----------|--------|
| 1 | Classique Cutz | Kitchener, ON | [`sites/classique-cutz`](sites/classique-cutz) |
| 2 | Tamil Saloon (Best Barbers) | Croydon, England | [`sites/tamil-saloon`](sites/tamil-saloon) |
| 3 | Plan B Barbershop | League City, TX | [`sites/plan-b-barbershop`](sites/plan-b-barbershop) |
| 4 | A1 Barbers | Croydon, England | [`sites/a1-barbers`](sites/a1-barbers) |
| 5 | Ranya Barber Croydon | Croydon, England | [`sites/ranya-barber`](sites/ranya-barber) |
| 6 | Barber Lab | Ajax, ON | [`sites/barber-lab`](sites/barber-lab) |
| 7 | Addiscombe Barbers | Croydon, England | [`sites/addiscombe-barbers`](sites/addiscombe-barbers) |
| 8 | Ellis's Barbershop | Croydon, England | [`sites/ellis-barbershop`](sites/ellis-barbershop) |
| 9 | Tony & Peter | Croydon, England | [`sites/tony-peter`](sites/tony-peter) |
| 10 | Hair and Beard | Ajax, ON | [`sites/hair-and-beard`](sites/hair-and-beard) |
| 11 | Distinguished Gents | Toronto (Etobicoke), ON | [`sites/distinguished-gents`](sites/distinguished-gents) |
| 12 | Valentino's Barbers | Croydon, England | [`sites/valentinos-barbers`](sites/valentinos-barbers) |
| 13 | Rozel Barbers | South Croydon, England | [`sites/rozel-barbers`](sites/rozel-barbers) |
| 14 | Magic Scissors | South Croydon, England | [`sites/magic-scissors`](sites/magic-scissors) |
| 15 | Gujarati Barber Hair Salon | Thornton Heath, England | [`sites/gujarati-barber`](sites/gujarati-barber) |
| 16 | Razor Sharp Barbershop | La Marque, TX | [`sites/razor-sharp-barbershop`](sites/razor-sharp-barbershop) |
| 17 | Scissorhands Barbershop | League City, TX | [`sites/scissorhands-barbershop`](sites/scissorhands-barbershop) |
| 18 | Gentlemen's Cut Barber Shop | Waterloo, ON | [`sites/gentlemens-cut`](sites/gentlemens-cut) |
| 19 | Extraordinary Premium Barber & Beauty | Croydon, England | [`sites/extraordinary-premium`](sites/extraordinary-premium) |
| 20 | Jacobs Barbers | Etobicoke, ON | [`sites/jacobs-barbers`](sites/jacobs-barbers) |
| 21 | By The Blade Barbers | Ajax, ON | [`sites/by-the-blade-barbers`](sites/by-the-blade-barbers) |

## Structure

```
.
├── README.md
└── sites/
    ├── <shop-slug>/
    │   └── index.html
    └── ...
```

Each `index.html` is fully self-contained: styles are inlined, fonts load from Google Fonts, and the only external calls are to Google Maps embeds (for the location section) and Google Fonts. No build tooling, package.json, or server is required.

## Viewing locally

Open any `sites/<shop-slug>/index.html` directly in a browser, or serve the whole repo:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000/sites/<shop-slug>/
```

## Deploying with GitHub Pages

1. Push this repo to GitHub (see below).
2. In the repo settings, enable **GitHub Pages** for the `main` branch, either from the root or a `/docs` folder.
3. Each site will then be reachable at `https://<username>.github.io/<repo-name>/sites/<shop-slug>/`.

To publish a single shop's site at the repo root instead (e.g. for a custom domain per shop), copy that shop's `index.html` into a separate repo's root.

## Pushing to GitHub

This folder is already an initialized git repository with an initial commit. To push it to your own GitHub repo:

```bash
git remote add origin https://github.com/<your-username>/<your-repo-name>.git
git branch -M main
git push -u origin main
```

## License

Concept designs only. Business names, addresses, and review excerpts belong to their respective owners and are used here for illustrative/preview purposes.
