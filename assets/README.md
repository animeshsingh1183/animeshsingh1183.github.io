# Website assets

## Profile photograph

The homepage currently loads your **GitHub account avatar** directly. This keeps the portrait in sync with your GitHub profile.

To use a separate, high-resolution photograph:

1. Save your image at `assets/profile.jpg` (recommended: square JPEG, at least 600 × 600 pixels).
2. In `index.qmd`, change the `<img>` tag's `src` to `assets/profile.jpg`.
3. Run `quarto preview` to check the framing.

Do not upload a photograph you do not have permission to publish.

A PDF CV can also be placed at `assets/cv.pdf` when ready.