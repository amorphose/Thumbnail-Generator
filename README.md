# Thumbnail Generator

A browser-based batch thumbnail generator. Drop images in, get a zip of resized, center-cropped square thumbnails out. No server, no uploads — everything runs client-side.

## Features

- **Drag-and-drop** or click-to-browse file selection
- **Center-crop to square** — handles any aspect ratio
- Configurable **max width**, **quality**, and **output format** (JPEG, WebP, PNG)
- Processes hundreds of images with a progress bar and live previews
- Downloads all thumbnails as a single **zip file** (via JSZip)
- Zero dependencies beyond [JSZip](https://stuk.github.io/jszip/) (loaded from CDN)

## Usage

Open `thumbnail-generator.html` in any modern browser. That's it.

1. Set your desired max width (default 300px), quality (default 70%), and format.
2. Drop image files onto the page or click to browse.
3. Click **Download Thumbnails (.zip)** when processing completes.

The zip contains a `thumbs/` folder with all generated thumbnails.

## Why

Built to batch-generate gallery thumbnails for [Aperture Cosmology](https://aperturecosmology.com) — specifically the Laniakea Field Guide's image grids, where full-resolution source images needed lightweight square crops for fast page loads.

## License

MIT — see [LICENSE](LICENSE).
