# Taylor Swift · Vinyl Room

A browser-based record gallery that turns ten Taylor Swift albums into an interactive WebGL carousel. Drag the collection into view, choose a record, and preview a track from that album in the iTunes catalog.

> **Gallery preview**  
> A screenshot of the finished listening room will appear here.

<!--
To add a screenshot where the placeholder appears, upload
docs/vinyl-room-preview.png and replace the placeholder above with:

![The Vinyl Room, showing record sleeves arranged around a lit WebGL carousel](docs/vinyl-room-preview.png)
-->

## Inside the room

- **A real 3D carousel.** Ten modeled sleeves and vinyl discs orbit on a fixed-camera stage with warm and violet lighting. Browse with drag, touch, the scroll wheel, or the on-screen controls.
- **Play from the collection.** Three.js raycasting selects a record. The disc spins as its preview plays, and the player shows the track name, progress, and pause control. The carousel advances when the preview ends, with playback capped at 30 seconds.
- **Live iTunes catalog data.** The page requests album artwork and official preview URLs at runtime and links to the corresponding iTunes Store item. The repository bundles no audio files or album images.

## Technology

| Layer | Tools |
| --- | --- |
| Scene | Three.js, WebGLRenderer, and Raycaster |
| Interface | Semantic HTML, native CSS, and vanilla JavaScript |
| Audio and artwork | HTML5 Audio and the iTunes Search API |
| Delivery | A single static HTML file with a CDN import map |

## Run locally

1. Download this repository or clone it, then open a terminal in the folder containing `index.html`.
2. Start a local server with Python 3.

   ```sh
   python -m http.server 8000
   ```

   On Windows, use `py -m http.server 8000` if `python` is unavailable. On macOS or Linux, `python3 -m http.server 8000` is another option.

3. Open [localhost:8000](http://localhost:8000) in a WebGL-enabled browser. Click a record to start playback. Internet access is required for the Three.js CDN and Apple catalog requests.

No build step, backend, API key, or package installation is required. To publish with GitHub Pages, set the source to **Deploy from a branch → main → /(root)**.

## Media and attribution

An independent fan project. Preview audio and cover artwork are provided courtesy of iTunes and are subject to Apple's promotional-content terms. The preview streams and artwork are separate from the project's source code. See [Apple's iTunes Search API terms](https://performance-partners.apple.com/search-api).
