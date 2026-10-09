# Arash Khajeh: personal website

A static site (one `index.html`, no build step) that you can host on GitHub Pages.

## Publish on GitHub Pages

1. Sign in to GitHub with your **personal** account, not a TRI organization.
2. Create a new **public** repository named exactly `arash-khajeh.github.io`.
3. Upload everything in this folder (`index.html`, `images/`, `.nojekyll`, this README), using **Add file → Upload files** or `git push`.
4. Go to **Settings → Pages**. Under *Build and deployment*, choose **Deploy from a branch**, then select `main` and `/ (root)`.
5. After a minute or two the site is live at `https://arash-khajeh.github.io`.

Optional custom domain (for example `arashkhajeh.com`): buy the domain, add it under **Settings → Pages → Custom domain**, create the DNS records GitHub lists, and turn on **Enforce HTTPS**.

## Personalize

- **Headshot:** save your photo as `images/headshot.jpg` (a 4:5 portrait crop, about 800×1000 px). If `headshot.jpg` is missing, an "AK" monogram shows instead.
- **Share card:** `images/share-card.png` (1200×630) is the preview shown when your link is posted on LinkedIn, Slack or X. It points to `https://arash-khajeh.github.io/`. If you move to a custom domain, update the `og:image`, `og:url` and `canonical` lines in `index.html`.
- **CV:** add `cv.pdf` to this folder, then uncomment the CV button in `index.html` (search for `cv.pdf`).
- **GitHub profile:** if you want one linked, add another `<a class="btn" ...>` next to the LinkedIn button.
- **New paper:** copy one `<li class="pub" ...>` block in the Publications list and edit it. The `data-cat` value (`ai`, `trib` or `fea`) controls the filter. Set `data-sel="1"` to include it under "Selected." The filter counts in the buttons are typed in by hand, so update them too.
- **News:** edit the `<ul class="news">` list.
- **Audio summaries:** files live in `audio/` (MP3, 64 kbps mono). To add one, copy a `<div class="listen">` block in Selected work and change the `src` path, the length and the label.

## Audio credits

The two audio summaries in `audio/` were generated with Google NotebookLM from the published papers and are labeled as AI-generated on the page.

## Figure credits

The six Selected work images (`images/ill-*.jpg`) are illustrations generated with ChatGPT. They are decorative, not data; their alt text starts with "Illustration:" for screen-reader users.

Real results are one click away:

- **View results chart** (HHAI 2026 and *Digital Discovery* items): charts drawn for this site from Table 1 of the HHAI paper and Fig. 3 of the *Digital Discovery* paper.
- **View original figure** opens the published figures:
  - `images/dd2025-conductivity.jpg`: Fig. 3 from Khajeh et al., *Digital Discovery* 4, 11–20 (2025), CC BY-NC 4.0.
  - `images/npj2024-md-validation.jpg`: Fig. 4 from Yang et al., *npj Computational Materials* 10, 296 (2024), CC BY-NC-ND 4.0. It's resized only, not modified, which that license requires.
