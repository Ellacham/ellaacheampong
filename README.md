# Emmanuella Acheampong · Portfolio

Personal portfolio for Emmanuella Acheampong, a researcher and data scientist working at the intersection of artificial intelligence, cybersecurity and digital trust.

It is a static site (plain HTML, CSS and a little JavaScript), so GitHub Pages can host it with no build step.

## Structure

```
index.html            All page content (About, Research, Projects, Talks, Writing, Contact)
404.html              Page shown for broken links
assets/css/style.css  Styles: navy, steel, bronze and cream palette; Source Serif 4 + Source Sans 3 fonts
assets/js/main.js     Mobile menu and active nav link
assets/img/           Photos and social-share image
.nojekyll             Tells GitHub Pages to serve the files as they are
```

## Editing content

Everything visible on the site lives in `index.html`. Each section has an id (`about`, `research`, `projects`, `talks`, `writing`, `contact`). To add a talk, project or note, copy an existing `<li>` or `<article>` block in that section and change the text.

When you change `assets/css/style.css`, bump the `?v=` number on its `<link>` in `index.html` so browsers fetch the new styles right away.

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
