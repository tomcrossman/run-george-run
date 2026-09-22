# Run George, Run

A side-scrolling dash on two blades. One self-contained HTML file: no build step,
no dependencies, works offline.

George is the same character who turns up as the final rival in
[Fingaz](https://github.com/tomcrossman/fingaz) — hat, blond hair, blue eyes, and
a pair of carbon running blades that jump higher than legs do.

## Play

Open `index.html`, or visit the hosted version.

- **Tap** to jump. **Hold** for a bigger one.
- **Tap again in the air** for a blade boost — the second jump.
- **Swipe down** (or press ↓) to slide under anything flying low.
- Crates and spikes want jumping. Drones want sliding. Capybaras want collecting.

It gets faster the longer you last, and your best distance is kept on the device.

## Put it on the web with GitHub Pages

1. **Settings → Pages → Source: Deploy from a branch → `main` / `/ (root)` → Save.**
2. After a minute or two it's live at
   `https://<your-username>.github.io/run-george-run/`

### Once it's hosted

- **Add to home screen** on a phone and it opens fullscreen with its own icon.
- It keeps working with no signal, thanks to `sw.js`.

If you change the game, bump `CACHE` in `sw.js` and `APP_VERSION` in `index.html`
together — the version shows in the bottom corner, so you can tell what deployed.

## Files

| file | what it is |
| --- | --- |
| `index.html` | the whole game — art, sound, music and logic |
| `manifest.webmanifest` | makes it installable to a home screen |
| `sw.js` | offline cache |
| `icon-*.png` | app icons, rendered from the sprite |
