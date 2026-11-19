# Diet Soda — Pure Zero

A product landing page for a zero-sugar soda. A 3D can floats in the middle of the hero, flavor cards switch the whole theme from green to blue, and the page has ingredient, taste, eco and review sections plus working-looking order and contact dialogs.

Built by AI from a prompt found online. Copy it, open it, or paste it into your own AI and make it yours, with no need to build it from scratch.

## Features

- Interactive 3D can (drag to rotate) with floating 3D cherries and leaves
- Two flavors, **Diet Classic** and **Zero Lime**, that switch the background theme, the taste meters and the ingredient text
- Sections for ingredients, taste profile, eco facts and reviews
- Order dialog with flavor, pack size, quantity and live total
- Contact dialog with a simple validation message
- Floating bubble background, glass-style header that appears on scroll
- Responsive layout and support for reduced-motion settings

## Tech

HTML, CSS and JavaScript, plus:

- [GSAP](https://gsap.com) and ScrollTrigger `3.12.2` (from cdnjs)
- [`<model-viewer>`](https://modelviewer.dev) for the 3D models (from unpkg)

No build step and no dependencies to install.

## Setup

**Option 1: just open it.** Double-click `index.html`. You need an internet connection.

**Option 2: run a local server** (needs [Node.js](https://nodejs.org)):

```bash
npm start
```

Then open the address it prints, usually http://localhost:3000.

**Put it online for free:** push this folder to GitHub, then go to Settings → Pages and deploy from the `main` branch.

## Make it yours

Open `index.html` and change:

| What | Where |
|---|---|
| Product name, flavors, prices | the hero cards (`data-flavor`) and the order dialog |
| Hero text | the `main-title` and `side-title` headings |
| Ingredients, nutrition pills | the `#ingredients` section |
| Taste meters | the `data-value-classic` and `data-value-blue` values |
| Eco stats | the `#eco` section |
| Reviews | the `#reviews` section |
| Colors | the CSS variables at the top of the `<style>` block |
| 3D model | the `src` on `<model-viewer id="product-model">` |

Quick way: paste `index.html` into your AI and say what you want, for example *"Turn this into an energy drink brand called VOLT with three flavors and new copy."*

## Good to know

- **Hosted files.** The 3D models and can images load from `api.getlayers.ai`:
  - `deit_soda2.glb` (the main can)
  - `cherry.glb`, `leaves.glb`, `blueberry.glb`
  - `Green Soda.png`, `Blue Soda.png`
  - `bubble.png`, `green base color.jpg`, `blue base color.jpg`

  If that host removes them, the 3D scene and images disappear. To make it fully offline, download them into an `assets/` folder and update the URLs in `index.html`, if the license allows.
- **Front-end only.** "Add to Bag" and "Send Message" don't send anything anywhere. They only show a confirmation message.
- **Demo content.** The brand, the prices, the reviews (names and cities), the "4.9 / 5.0 from 2,400+ Verified Reviews" rating, the "Design Awards" badge and the eco numbers are all placeholders. Replace them before using this for anything real.

## Credits

Original prompt: _add the source link here_
