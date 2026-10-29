# FORM website

A single-page static site for FORM, campaign planning and measurement software. There is no build step and no dependencies.

Live site: https://kayozhang1204-design.github.io/form-website/

Every push to `main` redeploys the site through GitHub Pages within a minute or two.

## Page structure

The page tells one story, and each section ends with a link to the next:

1. **Hero:** what FORM does, with a "Request a demo" button.
2. **The problem:** three costs of running campaigns across separate tools.
3. **How it works:** the four-step workflow (plan, create, launch, measure) and the screens a campaign reaches.
4. **Results:** the three outcomes teams can measure.
5. **Example:** a sample campaign for a made-up brand, with a video player and the four steps below it.
6. **Why now:** market figures from IAB's September 2026 outlook, with a source link.
7. **Video:** hidden until a video is added (see below).
8. **Get started:** the demo request.

## Before launch: set the contact email

The demo button uses the placeholder address `hello@form.example`. Search `index.html` for `form.example` and replace it with your real address.

## Sample scenario video

The Example section has its own video player. In `index.html`, find `EXAMPLE_VIDEO` and set `src` to a YouTube or Vimeo link, or to an MP4 path such as `videos/sample-scenario.mp4`. Add a `duration` such as `2:30` to show it on the play button. Until `src` is set, the photo shows a play button, and clicking it displays "The scenario video is coming soon."

## Adding videos

Edit the `VIDEOS` list near the end of `index.html`. The Video section and its menu link appear automatically once at least one entry has a `src`.

- **YouTube or Vimeo:** paste the normal share link into `src`. This is the best option for larger files.
- **Your own MP4:** add it to a `videos/` folder and set `src` to `videos/name.mp4`. GitHub rejects files over 100 MB.
- **Captions and transcript:** add a `.vtt` file path to `captions`, and `["Speaker", "What they said"]` pairs to `transcript`.

## Photography

Photos are real stock images from Unsplash, used under the Unsplash License and credited in the footer. Replace them with your own team or customer photos when you have them, with permission.

## Accessibility

Text colours meet WCAG AA contrast. The page has a skip link, a keyboard-operable mobile menu, visible focus outlines, alt text on every photo, one h1 with ordered headings, and reduced-motion support.

## Run locally

```sh
python3 -m http.server 8000
```

Then open http://localhost:8000.
