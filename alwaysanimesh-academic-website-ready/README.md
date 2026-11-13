# Academic website — Animesh Singh

A Quarto-based academic homepage and technical blog, configured for:

- GitHub account: `alwaysanimesh`
- Repository: `alwaysanimesh/alwaysanimesh.github.io`
- Planned URL: <https://alwaysanimesh.github.io>

## Status: source only, not published

**Publishing is intentionally disabled.** The proposed GitHub Actions workflow is saved as
`deployment/publish.yml.example`, which GitHub will not execute automatically.
No GitHub Pages settings are included in this project. The Quarto site's
`site-url` identifies the eventual address; it does not publish the website.

**Note:** A public GitHub repository makes the **source files** publicly readable,
even before GitHub Pages is turned on. Review text before uploading anything sensitive.

## Review before publication

1. Confirm biography, research directions, publications and experience descriptions.
2. Add an email address only if you want it public. Contact currently links to GitHub only.
3. Replace the sample blog post with your own content; it is marked `draft: true`.
4. Optionally add a portrait and CV PDF (only if you want them public).
5. Confirm the publication links and other external URLs.

## Local preview

Install [Quarto](https://quarto.org/docs/get-started/) and run from this directory:

```bash
quarto preview
```

Other optional tools: Git, VS Code.

## Create the repository

Open <https://github.com/new?name=alwaysanimesh.github.io>.
Create a **public** repository called **alwaysanimesh.github.io**, owned by
**alwaysanimesh**. Leave README, .gitignore and license unchecked.

To upload from Git after the repository exists:

```bash
git init
git branch -M main
git add .
git commit -m "Add Quarto academic website starter"
git remote add origin https://github.com/alwaysanimesh/alwaysanimesh.github.io.git
git push -u origin main
```

Alternatively, ChatGPT can upload these text files through a connected GitHub app
once the repository has been created and granted access.

## Publish later, after review

When you want the website live:

1. Copy `deployment/publish.yml.example` to `.github/workflows/publish.yml`.
2. Grant Actions `Read and write permissions` under Settings → Actions → General if needed.
3. Push to `main` to run the workflow, which builds the Quarto website and creates
   or updates the `gh-pages` branch.
4. Configure Settings → Pages → Build and deployment → Deploy from a branch,
   selecting `gh-pages` and `/ (root)`.
5. Verify the live site at <https://alwaysanimesh.github.io>.

See the [Quarto GitHub Pages guide](https://quarto.org/docs/publishing/github-pages.html).

## Writing blog posts

Each blog post resides in `posts/<slug>/index.qmd`. Start by copying the example
in `posts/hello-world/`, editing the YAML metadata and content, and keeping
`draft: true` until it is ready. Remove the flag when you want it published.

## Site files

- `_quarto.yml`: overall website configuration
- `index.qmd`: homepage
- `research.qmd`: research directions
- `publications.qmd`: publication list
- `blog.qmd`: blog listing
- `posts/`: Markdown/Quarto blog posts
- `cv.qmd`: CV and experience summary
- `contact.qmd`: public contact links
- `styles.css`: theme adjustments
- `deployment/publish.yml.example`: disabled publishing workflow template
