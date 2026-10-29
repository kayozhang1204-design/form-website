# FORM website

A static website with no build step or dependencies.

## Files

- index.html: complete page, including CSS, JavaScript, inline SVG graphics, and animations.
- .nojekyll: serves the site as plain static files on GitHub Pages.

## Run locally

Open index.html in your browser, or run:

```sh
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Publish on GitHub Pages

1. Extract this ZIP.
2. Upload index.html and .nojekyll to the root of your GitHub repository. You can also include this README.
3. In the repository, open Settings > Pages.
4. Under Build and deployment, choose Deploy from a branch.
5. Select your main branch and / (root), then save.
6. Once deployment finishes, GitHub shows the published URL in Settings > Pages.

Upload the extracted files, not the ZIP itself. No npm install or build command is needed.

## Editing

Styles are in the style block and behavior is in the script block in index.html. Graphics are drawn with inline SVG and CSS, so there is no separate images directory.

The Field Notes case study is an illustrative example, not a claim of actual customer results.
