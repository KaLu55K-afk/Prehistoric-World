# Prehistoric World — Digital Museum

A responsive, static educational website about prehistoric life, fossils, geological time, and human evolution. It is designed for GitHub Pages.

## Files
- `index.html` — page structure and educational sections
- `style.css` — responsive visual design
- `script.js` — searchable encyclopedia, navigation, and 3D model loader

## Run locally
1. Extract this folder.
2. Open `index.html` in a modern browser.
3. An internet connection is needed for the 3D viewer library and optional web fonts.

For the most reliable local preview, run a small local web server (for example, VS Code's Live Server extension).

## Publish on GitHub Pages
1. Create a repository on GitHub.
2. Upload `index.html`, `style.css`, `script.js`, and `README.md` to the repository's root.
3. Open **Settings → Pages**.
4. Under build and deployment, choose **Deploy from a branch**, select `main` and `/(root)`, then save.
5. Wait for deployment. The address is usually `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`.

## Add more encyclopedia entries
In `script.js`, add another object to the `entries` array. Example:

```js
{
  name: "Species name",
  category: "dinosaur", // dinosaur, plant, creature, human, fossil
  icon: "🦴",
  period: "Geological period and approximate dates",
  summary: "Short overview.",
  details: "Longer information about anatomy, environment, evolution, discovery, and evidence."
}
```

Keep claims evidence-based and use approximate dates when science is uncertain. Add citations and source links to entries as the archive grows.

## Add 3D models
The 3D viewer accepts a direct public URL to a `.glb` or `.gltf` file. Enter the URL and specimen name in the **3D museum** section. The model host must allow public access and embedding/CORS as required by the browser.

This ZIP does **not** contain a full library of dinosaur, plant, fossil, or animal models. Each model must be sourced individually, and its license must permit the intended use. Keep attribution and license information with every asset. Do not assume a model is free to reuse just because it can be viewed online.

## Scientific scope
This is a substantial starter site, not a literally complete inventory of every organism that ever lived. Many extinct species are undiscovered, and many are known only from incomplete fossils. Treat dates and interpretations as approximate where appropriate.
