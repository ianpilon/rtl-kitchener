# RTS Kitchener

Static site for Refrigerated Transport Service (1620 Strasburg Rd, Kitchener, ON).

Single-file HTML with inline CSS, no build step. Open `index.html` in a browser.

## Layout

```
rtl-kitchener/
├── index.html        # the whole site
└── assets/           # drop real images here (see assets/README.md)
```

## How image swap-in works

Every `<img>` points at `assets/<name>.<ext>`. If the file is missing, the image
falls back to a `placehold.co` placeholder via the `onerror` attribute, so the
page renders cleanly with or without real assets. To swap in a real image, just
save the file at the path the HTML expects — no code change needed.

See `assets/README.md` for the full list of slot names and target dimensions.

## Local preview

```sh
# anything that serves the directory works; e.g. python:
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy

GitHub Pages is enabled on `main` / root. Pushes to `main` deploy automatically.
