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

The site is published from the root of the main branch at https://kayozhang1204-design.github.io/the-creation-machine/. Every push to main redeploys it automatically within a minute or two. No npm install or build command is needed.

## Adding videos

The Video briefings section is driven by the `VIDEOS` list near the end of the script block in index.html. Each entry has a label, title, speakers, duration, summary, `src`, an optional `poster` image, an optional `captions` file, and an optional `transcript`.

- **YouTube or Vimeo:** paste the normal share link into `src`, for example `https://youtu.be/VIDEO_ID`. This is the best option for long or large videos.
- **Your own MP4:** add the file to a `videos/` folder and set `src` to `videos/name.mp4`. Keep files well under GitHub's 100 MB per-file limit.
- **Transcript:** add lines as `['Speaker name', 'What they said']` pairs. A "View transcript" toggle appears automatically.

An entry with an empty `src` shows as "Coming soon". The first entry is the featured video.

## Photography

People photos are loaded from Unsplash under the Unsplash License, and the photographers are credited above the footer. The people shown are models, not customers or staff. Replace them with your own team or customer photos when you have them, with permission.

## Editing

Styles are in the style block and behavior is in the script block in index.html. Graphics are drawn with inline SVG and CSS, so there is no separate images directory.

The Field Notes case study is an illustrative example, not a claim of actual customer results.
