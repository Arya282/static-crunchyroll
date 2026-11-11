# Static Crunchyroll Landing Page

A practice project that recreates the look of a streaming-service landing page, built with plain HTML, CSS, and a small amount of vanilla JavaScript. It has no build step and no dependencies.

**Live demo:** https://clonechyroll.netlify.app

> This is a personal learning exercise. It isn't affiliated with or endorsed by Crunchyroll. All trademarks, logos, and artwork belong to their owners.

## Features

- **Navigation bar** with a logo and "Log In" / "Start Free Trial" buttons that change on hover.
- **Hero banner** with a background image, a "New Dubs" announcement, and a **Compare Plans** button that scrolls smoothly down to the pricing section.
- **"Pick Your Premium" pricing section** with three plan cards (Fan, Mega Fan, Ultimate Fan). The middle "Most Popular" card is highlighted.
- **Monthly / Yearly billing toggle**: switching it swaps every card's price between monthly and yearly. The prices are stored in `data-monthly` and `data-yearly` attributes.
- **Responsive layout**: below 950px wide, the cards stack in a single column.
- Google Fonts: DM Sans, Oxanium, and Happy Monkey.

## Project Structure

```
.
├── netlify.toml              # Netlify config: publishes the "Practice Project" folder
└── Practice Project/
    ├── index.html            # Page markup and the billing-toggle script
    ├── styles.css            # All styling, including the responsive rule
    ├── Crunchyroll-Logo.png  # Logo in the nav bar
    ├── clover.png            # Logo shown in the banner
    ├── clover.jpg            # Alternate banner image (currently unused)
    └── asta.png              # Banner background artwork
```

## Running Locally

You don't need to install anything. Either:

- open `Practice Project/index.html` directly in a browser, or
- serve the folder with any static server, for example:

  ```bash
  npx serve "Practice Project"
  # or
  python3 -m http.server --directory "Practice Project" 8000
  ```

## Deployment

The site is deployed on [Netlify](https://www.netlify.com/). `netlify.toml` sets the publish directory to `Practice Project`, and Netlify deploys that folder as-is with no build command. A push to `main` starts a new production deploy.

## Tech Stack

- HTML5
- CSS3 (Flexbox, Grid, media queries, transitions)
- Vanilla JavaScript
- Netlify (hosting)
