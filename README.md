# Yitian Wei — Portfolio Website

A four-page portfolio site in plain HTML & CSS. No build tools, no frameworks.
Brand system: cobalt blue (#093180), off-white (#FFFEFA), Quicksand — matching the
Personal Identity project, so the whole site is on-brand.

## Pages
```
portfolio/
├── index.html                      ← Home / Work (landing page)
├── about.html                      ← About Me
├── work-personal-identity.html     ← In-depth case study (Personal Brand Identity)
├── work-alethia.html               ← ALETHIA magazine showcase   ✅ images done
├── work-bcspca.html                ← BC SPCA annual report showcase ✅ images done
├── css/styles.css                  ← all styling (brand colors at the top)
├── images/                         ← project images
└── Yitian_Wei_GraphicDesigner_2026.pdf  ← downloadable résumé
```

## What's already done
The **ALETHIA** and **BC SPCA** showcase pages are fully built — their images are already
in `images/` and embedded. Nothing to do there.

## What still needs your images
Two things still show striped placeholders. Drop the files into `images/` with the exact
names below, and they'll appear automatically.

### 1. Personal Identity visuals (from your Canva brand book)
In Canva: **Share → Download → PNG → All pages**, then rename the pages you want:

| Canva page | Save as |
|-----------|---------|
| Cover ("Personal Identity") | `images/identity-hero.png` |
| Brand Discovery moodboard | `images/identity-moodboard.png` |
| Logo Development (final) | `images/identity-logo.png` |
| Color Scheme | `images/identity-color.png` |
| Brand Typography | `images/identity-type.png` |
| Stationery Suite | `images/identity-stationery.png` |

Also save the logo page (or cover) as `images/work-identity.jpg` for the home-page
thumbnail. (The colour swatches on the case-study page are already coded by hand, so
those will look right even before you add the color image.)

### 2. Your photo (About page)
Save a professional photo as `images/portrait.jpg` (around 900 × 1200 px, portrait).

### How to switch a placeholder to a real image
In the HTML you'll see, under each placeholder:
```html
<div class="ph"> ... </div>
<!-- <img src="images/identity-logo.png" alt="yw logo" /> -->
```
Delete the `<div class="ph"> ... </div>` line and remove the `<!--` / `-->` around the `<img>`.

## Changing brand colors
Open `css/styles.css` → the `:root { }` block at the top. Your three brand colors are
already set as `--accent`, `--accent-2`, and `--paper`.

## A couple of things to personalize
- The **Reflection** on the Personal Identity page is built from your own discovery notes —
  tweak it to sound even more like you (look for the `✏️` note).

## Going live with GitHub Pages
1. Create a repo named `yitianw.github.io` (Public).
2. Upload the **contents** of this `portfolio/` folder (so `index.html` sits at the root).
3. Settings → Pages → Deploy from branch → `main` → `/ (root)` → Save.
4. Your site goes live at `https://yitianw.github.io` in a minute or two.

To preview locally, just double-click `index.html`.
