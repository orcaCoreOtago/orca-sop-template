# ORCA SOP template

Starting point for a new ORCA standard operating procedure. Every SOP is its own repository, published at `https://orcacoreotago.github.io/<repo-name>/` and listed on the hub site at <https://orcacoreotago.github.io/>.

## Start a new SOP

1. On this repository's GitHub page click **Use this template → Create a new repository**. Owner `orcaCoreOtago`, a short lowercase name ending in `-sop` (e.g. `itrax-startup-sop`), **Public**.
2. In the new repository: **Settings → Pages → Build and deployment → Source: GitHub Actions**.
3. Clone it (RStudio: *File → New Project → Version Control → Git*) and in `_quarto.yml` change `REPO-NAME` in `repo-url` to the new repository's name.
4. Write the SOP in `index.qmd`. Put pictures in `images/`.
5. Preview with `quarto preview` (or the **Render** button in RStudio).
6. Commit and push. GitHub renders the web page and PDF automatically; watch progress on the **Actions** tab. First publish takes 2–3 minutes.
7. Add the SOP to the hub: edit `sops.yml` in the `orcaCoreOtago.github.io` repository (it can be done in the GitHub web editor) and commit. The home page card and navbar menu appear automatically.

## Rules

- Never commit passwords, connection files, or anything that should not be public. GitHub Pages sites are public.
- Keep `_quarto.yml` identical across SOPs apart from `repo-url`, so they all look the same.
- Don't commit `_site/`; GitHub builds it.
