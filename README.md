# MG Browser Web 🌐

**MG Browser Web** is the web-based companion project for MG Browser. It is intended to be published with GitHub Pages and opened inside an existing web browser.

## Project structure

```text
MG-Browser-Web/
├── index.html
├── README.md
├── favicon.svg
└── images/
    ├── .gitkeep
    └── mg-browser-icon.svg
```

- **`index.html`** — Main page. Add the HTML, CSS, and JavaScript for the interface here.
- **`images/`** — Store backgrounds, logos, and other image assets here.
- **`images/mg-browser-icon.svg`** — MG Browser icon artwork.
- **`favicon.svg`** — Icon displayed in the browser tab.

## Add the favicon

Place this line inside the `<head>` section of `index.html`:

```html
<link rel="icon" href="./favicon.svg" type="image/svg+xml">
```

## Use images

Keep image files in the `images/` folder and reference them with relative paths, for example:

```css
body {
  background-image: url("./images/background.jpg");
}
```

Make sure the image filename and extension match the uploaded file.

## Publish with GitHub Pages

1. Open the repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select the `main` branch and the `/ (root)` folder, then save.
4. After deployment finishes, open the published URL shown in the Pages settings.

Expected URL format:

`https://smm2318.github.io/MG-Browser-Web/`

## Important note

This repository hosts a **web page**, not a standalone browser engine or Windows application. A GitHub Pages version can provide a custom home page and send searches to a search engine, but browser tabs and unrestricted navigation to arbitrary websites cannot be fully controlled from an ordinary web page because of browser security restrictions.

The separate Windows app can later reuse this design and be packaged with a desktop framework such as Electron.

## Project status

- [x] Create the `images/` folder
- [x] Add MG Browser SVG icon
- [x] Add website favicon
- [ ] Add the main `index.html` design
- [ ] Publish and test with GitHub Pages

---

Made for the **MG Browser** project.
