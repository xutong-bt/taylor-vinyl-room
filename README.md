# Taylor Swift Vinyl Room

An independent fan project that turns Taylor Swift’s album catalog into an interactive vinyl room. Explore the eras, listen to official previews, and build a collection you can turn into a poster.

[Open the Vinyl Room](https://xutong-bt.github.io/taylor-vinyl-room/)

## Inside the room

| Area | What you can do |
| --- | --- |
| **Home** | Drag through a Three.js carousel of 10 featured records, or browse them with the arrow controls. A 2D gallery is available if the 3D scene cannot start. |
| **Player** | Play, pause, and replay available Apple previews in a player shared across the site. A preview stops when it ends or reaches 30 seconds. |
| **Explore** | Search, filter, and sort 16 albums: 12 original studio albums and four Taylor’s Version re-recordings. |
| **Album Detail** | Open a direct album link, browse the tracks returned by Apple, select an available preview, and follow the official Apple link when available. |
| **My Collection** | Save favorite albums in this browser, see the collection breakdown, and filter or sort your library. |
| **Share** | Export a collection poster as a PNG in portrait, square, or landscape format, or share a link to a snapshot. Recipients can view the snapshot before choosing whether to copy albums into their own collection. Native sharing is available on supported browsers. |

## Built with

- HTML, CSS, and vanilla JavaScript
- Three.js and WebGL for the vinyl carousel
- Apple iTunes API for album artwork, track metadata, and official previews
- Canvas for poster export, localStorage for favorites, and URL fragments for navigation

The site runs as a single HTML file and is hosted on GitHub Pages. This fan project is unaffiliated with Taylor Swift or Apple. Artwork and audio remain the property of their respective rights holders.

## Run locally

1. Download or clone the repository.
2. Open a terminal in the folder that contains `index.html`.
3. Run `python -m http.server 8000`.
4. Open the local server at `http://localhost:8000/` in your browser.

An internet connection is needed for Three.js, Apple artwork, and audio previews. The album catalog is bundled with the page.

## Screenshots

Screenshots can be added here under `docs/screenshots/` once they are captured for this release.
