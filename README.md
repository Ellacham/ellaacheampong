# Emmanuella Acheampong · Portfolio

Personal portfolio for Emmanuella Acheampong, a researcher and data scientist working at the intersection of artificial intelligence, cybersecurity and digital trust.

It is a static site (plain HTML, CSS and a little JavaScript), so GitHub Pages can host it with no build step.

## Structure

```
index.html            All page content (About, Research, Projects, Speaking, Insights, Contact)
assets/css/style.css  Styles and colour palette (navy, white, cool grays, one blue accent)
assets/js/main.js     Mobile menu, active nav link, scroll reveal
assets/img/           Photos, logo, favicon and social-share image
.nojekyll             Tells GitHub Pages to serve the files as they are
```

## Editing content

Everything visible on the site lives in `index.html`. Each section is marked with a comment (`<!-- Projects -->`, `<!-- Speaking -->`, …). To add a talk, project or post, copy an existing `<li>` or `<article>` block in that section and change the text.

## Publishing with GitHub Pages

The live site is at https://ellacham.github.io/ellaacheampong/, served from the `main` branch of this repository.

To set it up again from scratch:

1. Push this folder to a GitHub repository.
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose `main` and `/ (root)`, then save.
4. The site will appear at `https://<your-username>.github.io/<repository-name>/` after a minute or two.

To use the custom domain `ellaacheampong.com` instead, enter it under **Settings → Pages → Custom domain** and point the domain's DNS at GitHub Pages ([GitHub's guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)).

## Previewing locally

Open `index.html` in a browser, or run a small local server from this folder:

```bash
python3 -m http.server 8000
```

then visit http://localhost:8000.
