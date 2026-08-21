# zaineb-ibork.github.io

Personal academic site — Zaineb IBORK, postdoctoral researcher in 3D computer vision, NII Tokyo.

## Files

| File | What it is |
|------|-----------|
| `index.html` | The whole site: HTML, CSS and JS in one file. No build step, no dependencies. |
| `profile.jpg` | Portrait, pre-cropped square (720×720). Replace with any square image of the same name. |
| `CV_Zaineb_Ibork.pdf` | Linked from the "Download CV" button. Replace whenever you update it. |

## Publishing on GitHub Pages

1. Create a new **public** repository named exactly `Zaineb-Ibork.github.io`.
2. Upload `index.html`, `profile.jpg` and `CV_Zaineb_Ibork.pdf` to the root of the repository
   (Add file → Upload files → Commit changes).
3. Go to **Settings → Pages**. Under *Build and deployment*, set Source to
   *Deploy from a branch*, branch `main`, folder `/ (root)`. Save.
4. Wait a minute or two, then open **https://zaineb-ibork.github.io**.

Every later commit to `main` republishes the site automatically.

## Publication links

Titles link to the open-access record where one exists:

| Paper | Links to |
|-------|----------|
| Saliency Prediction on 3D Meshes (VCIP 2025) | hal-05399363 |
| Un indice d'evaluation sans reference (GRETSI'25) | hal-05230505 |
| No Reference 3D MQA from 2D Projections (IEEE Access) | doi.org/10.1109/ACCESS.2024.3435377 |
| A No Reference Deep QA Index for 3D Colored Meshes (SMC 2024) | IEEE Xplore 10831641 |
| Evaluation sans reference ... projections 2D (RFIAP 2024) | hal-04644716 |
| A Fully Automatic Colorimetric Saliency Detection (ISIVC 2024) | hal-04587801 |
| No Reference 3D MQA Using Deep Convolutional Features (ISPA 2023) | hal-04263475 |

Three entries are intentionally unlinked: the two 2026 papers (ACIVS, S+SSPR) are accepted but
not yet published, and the Nouri-first GRETSI'25 saliency paper has no HAL record yet. To add a
link later, wrap the title exactly like the others:

```html
<p class="pub-title"><a href="URL" target="_blank" rel="noopener">Title</a>
  <a class="src" href="URL" target="_blank" rel="noopener">HAL</a></p>
```

Note: your CV cites hal-04644716 for the GRETSI'25 paper, but that ID belongs to the RFIAP 2024
paper. The correct GRETSI'25 ID is hal-05230505 — worth fixing in the PDF too.

## Editing

Open `index.html` in any text editor. Colours live in the `:root` block at the top —
change one value there and it updates everywhere.

To add a publication, copy an existing `<li>` block inside `<ol class="pubs">` and edit it.
Wrap your own name in `<span class="me">Z. Ibork</span>` to keep the red highlight.

## Notes

- The hero animation is a subdivided icosahedral mesh coloured by a synthetic saliency field.
  It stops automatically for visitors who have "reduce motion" enabled, and pauses on hidden tabs.
- Your phone number and date of birth are deliberately not on the page — both are fine on a CV
  sent to a named recipient, but neither belongs on a public URL that gets scraped.
