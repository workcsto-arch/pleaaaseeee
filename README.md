# NTU Radio — Responsive RF / Varactor Tuner Lab

A GitHub-ready version of the NTU Radio interactive lab. The portrait/mobile layout is included.

## Files

- `index.html` — main interactive lab page
- `assets/audio/` — compressed MP3 files used by the radio playlist

Audio is stored as separate files instead of being embedded in the HTML, keeping the project smaller and making it easier to host on GitHub Pages.

## Run locally

For the most reliable audio loading, serve this folder through a local web server rather than opening `index.html` directly. For example, with Python:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.

## Publish with GitHub Pages

1. Create a GitHub repository and upload the contents of this folder (keep the `assets` folder beside `index.html`).
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and `/ (root)`, then save.
5. Wait for GitHub Pages to publish the site.

Do not upload only `index.html`; the audio playlist depends on the files in `assets/audio/`.
