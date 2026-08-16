# Chuck Joke

A purposefully pointless Chuck Norris joke dispenser and a compact showcase for [Unholy CSS](https://github.com/nphillips-dev/Unholy). It is for anyone who wants a quick laugh—or a tiny, dependency-free example of Unholy v3.1 in a real page.

[View the live site](https://chuckjoke.neocities.org/)

## Features

- Fetches a new Chuck Norris joke on page load and on demand.
- Falls back to a bundled set of jokes when the remote service is unavailable.
- Rotates through five local portraits.
- Supports the button or the <kbd>Space</kbd> key for another joke.
- Uses Unholy v3.1 layout, utility, theme, and animation styles.
- Adapts to mobile and desktop screens and respects reduced-motion preferences.

## Getting started

### Prerequisites

You only need a modern web browser. An internet connection is required for fresh jokes from the API, but the local fallback jokes still work without it.

### Installing

Clone the repository:

```sh
git clone https://github.com/nphillips-dev/chuckjoke.git
cd chuckjoke
```

There are no packages to install and no build step.

### Running locally

Open `index.html` directly in your browser. You can also serve the repository with any static web server if you prefer an HTTP URL.

## How it works

The project is deliberately small:

```text
chuckjoke/
├── core/
│   └── unholy-variables.css
├── images/
│   └── 1.jpg … 5.jpg
├── index.html
├── unholy-animations.css
├── unholy-core.css
└── unholy-utility.css
```

`index.html` contains the page structure, presentation overrides, and vanilla JavaScript. Fresh jokes come from the [Chuck Norris API](https://api.chucknorris.io/); the Unholy files provide the responsive grid, theme variables, utilities, and motion.

## Testing

The repository does not currently include an automated test suite. After changing the site, check that:

- The initial joke loads or a fallback appears.
- **Another one** changes both the joke and portrait.
- Pressing <kbd>Space</kbd> works when the page body has focus.
- The layout remains readable at mobile and desktop widths.
- All five files under `images/` remain available.

## Deployment

The site is entirely static. The current public version is hosted at [chuckjoke.neocities.org](https://chuckjoke.neocities.org/); this repository does not include automated deployment configuration.

## Built with

- Semantic HTML
- Modern CSS
- Vanilla JavaScript
- [Unholy CSS v3.1](https://github.com/nphillips-dev/Unholy)
- [Chuck Norris API](https://api.chucknorris.io/)

## Author

Created by [nphillips-dev](https://github.com/nphillips-dev).

## Acknowledgments

- The intentionally overpowered styling comes from [Unholy CSS](https://github.com/nphillips-dev/Unholy).
- Fresh internet folklore is supplied by the [Chuck Norris API](https://api.chucknorris.io/).
