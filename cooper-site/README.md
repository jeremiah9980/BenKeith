# Three minutes — the night strangers saved Cooper

Static site, no build step.

```
index.html
media/
  hero.jpg, poster.jpg
  three-minutes.mp4        (32 MB, 720p — compressed from the 127 MB original)
  stills/                  (24 frames from the video, full + thumbnail, with meta.json)
```

The Community Lifesaver Award video is embedded from YouTube (yp7syAZahhA), so it isn't in the repo.

## Publish on GitHub Pages

1. Create a public repo (e.g. `three-minutes`).
2. Upload `index.html` and the whole `media/` folder to the repo root. Everything is under GitHub's 100 MB per-file limit.
3. Settings → Pages → Deploy from a branch → `main` / `(root)` → Save.
4. Live in about a minute at `https://<user>.github.io/three-minutes/`.

Custom domain: add a `CNAME` file and point DNS at GitHub Pages.

## Editing

- **Cooper's thank you:** replace the dashed "pending" letter in `#thanks`.
- **Photos:** drop a frame in `media/stills/` and add a `<figure class="photo">` to any gallery grid; the lightbox picks it up automatically.
- **Names:** add another `<div class="story-card">` under The People.
- **Counter:** the live "Time Since 8:31 PM" counter is set in the script at the bottom (`crashDate`).

Check before publishing: the transcript in `#words` (a few words were hard to hear over the music), what the officer's title is (currently "the officer who worked the scene"), and the "stepdad" wording.
