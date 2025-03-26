# Wikipedia Smooth Scroll Userscript

A userscript that adds smooth scrolling to internal links on Wikipedia and its sister sites.

## Features

- 🚀 Buttery-smooth scrolling for all in-page links (`#anchor` links)
- 🔄 Full support for browser history (back/forward buttons)
- 🌐 Works across all Wikimedia Foundation sites:
  - Wikipedia
  - Wiktionary
  - Wikibooks
  - Wikiquote
  - Wikivoyage
  - Wikisource
  - Wikinews
  - Wikiversity
  - Wikifunctions
- ✨ Handles dynamically loaded content
- 🛠️ Pure JavaScript - no dependencies required

## Installation

1. Install a userscript manager:
   - [Tampermonkey](https://www.tampermonkey.net/) (recommended)
   - [Violentmonkey](https://violentmonkey.github.io/)
   - [Greasemonkey](https://www.greasespot.net/)

2. Click here to install:  
   [![Install](https://img.shields.io/badge/Install%20directly%20from-URL-brightgreen)](https://github.com/yourusername/wikipedia-smooth-scroll/raw/main/wikipedia-smooth-scroll.user.js)

   Or manually copy the script from the repository and add it to your userscript manager.

## How It Works

The script:

1. Intercepts clicks on internal links
2. Prevents the default "jump" behavior
3. Animates smooth scrolling to the target element
4. Handles edge cases like:
   - Special characters in anchor IDs

## Technical Details

- Uses `scrollIntoView` with `behavior: 'smooth'` for smooth animations
- Manages URL state to prevent native browser jumping
- Lightweight (less than 2KB without minification)

## Possible Issues

- Some extremely old browsers may not support the smooth animation (will fall back to instant scroll)

## License

MIT License - Free to use and modify
