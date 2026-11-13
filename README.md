# Animesh Singh — academic website

Source code for **https://animeshsingh1183.github.io**, built with [Quarto](https://quarto.org/).

## Pages

- `index.qmd`: homepage
- `research.qmd`: research overview
- `publications.qmd`: publications
- `blog.qmd`: blog listing
- `posts/`: individual blog articles written in Markdown/Quarto
- `cv.qmd`: CV
- `contact.qmd`: public contact information
- `styles.css`: website appearance

## Preview locally

Install Quarto, then run in the project root:

```bash
quarto preview
```

## Upload to GitHub

1. Extract this ZIP locally.
2. Open https://github.com/animeshsingh1183/animeshsingh1183.github.io
3. Upload the **contents of the extracted folder**, not the outer folder itself.
4. Confirm `_quarto.yml` and `index.qmd` appear at the repository root.

If updating an existing local clone, copy the extracted files into the clone instead, then commit and push.

## Publishing (not enabled yet)

The sample workflow is at `deployment/publish.yml.example` and is **inactive**. When you are ready:

1. Copy its contents into `.github/workflows/publish.yml`.
2. Commit and push to `main`.
3. In repository Settings → Actions → General, ensure workflows can write repository contents.
4. In Settings → Pages, select **Deploy from a branch**, using branch `gh-pages` and directory `/ (root)` after the workflow creates that branch.

Do not enable publishing until you are comfortable with the public content. Note that files pushed into a public repository are publicly visible even before GitHub Pages is enabled.

## Update public details

Before publishing, verify publication metadata, edit biography/CV/contact details, and add your preferred public email and CV PDF if desired. The sample blog post is marked `draft: true`.
