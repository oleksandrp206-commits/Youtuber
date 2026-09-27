# Max Overdrive — Creator Landing Page

A single-page, animated landing page for a YouTube creator, built as one
self-contained HTML file (no build step, no dependencies to install).

## Features

- 5 full-screen sections with scroll-snap (`Hero`, `Latest videos`,
  `Find me elsewhere`, `Story`, `Collab / contact`) — great for quickly
  screenshotting each screen
- Scroll-triggered reveal animations that replay both scrolling down
  *and* scrolling back up (`IntersectionObserver`)
- Animated subscriber / video / views counters that count up on view
- Light / dark theme toggle
- English (default) / Russian language toggle, saved in `localStorage`
- Right-side dot pager to jump between the 5 screens
- Respects `prefers-reduced-motion`
- Zero build tools — just HTML, CSS and vanilla JS in one file

## Getting started

1. Clone or download this repo.
2. Open `index.html` directly in a browser — that's it, no install step.

## Deploying with GitHub Pages

1. Rename the site file to `index.html` if it isn't already, and make
   sure it's in the root of this repo (or in a `/docs` folder).
2. Go to **Settings → Pages** in this repository.
3. Under **Source**, choose the branch (e.g. `main`) and folder
   (`/root` or `/docs`), then save.
4. GitHub will publish the site at:
   `https://oleksandrp206-commits.github.io/Youtuber/`

## Customizing

All content lives in one file. To personalize it:

- Update the name, avatar initials, tagline and stats in the **Hero**
  section.
- Replace the placeholder video titles/thumbnail gradients in
  **Latest videos** with real ones.
- Swap the follower counts and links in **Find me elsewhere** for your
  real YouTube / Telegram / Instagram / TikTok / Twitch profiles.
- Edit the timeline entries in **Story** to match your own history.
- Update the contact email and Telegram handle in the **Collab**
  section.
- Both languages (English/Russian) live in a single `dict` object near
  the bottom of the `<script>` tag — edit the strings there to change
  copy in either language.

## Tech stack

- HTML5 + CSS (custom properties for theming, no framework)
- Vanilla JavaScript (`IntersectionObserver`, `requestAnimationFrame`
  for the counters)
- Google Fonts: [Fredoka](https://fonts.google.com/specimen/Fredoka) +
  [Plus Jakarta Sans](https://fonts.google.com/specimen/Plus+Jakarta+Sans)

## License

Feel free to use and adapt this template for your own creator page.
