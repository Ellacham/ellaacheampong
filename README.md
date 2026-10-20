# Emmanuella Acheampong · Portfolio

Personal portfolio for Emmanuella Acheampong, a researcher and data scientist working at the intersection of artificial intelligence, cybersecurity and digital trust.

It is a static site (plain HTML, CSS and a little JavaScript), so GitHub Pages can host it with no build step.

## Structure

```
index.html                     Homepage: About (bio, interests, education, honors, service), Research,
                               Projects, Publications, Talks, Writing, Contact
research/*.html                One overview page per study (linked from the Research cards)
projects/fraudlens.html        FraudLens technical page
assets/docs/                   Academic Resume PDF (opened by "Resume" and "Academic Resume")
assets/css/style.css           Styles for every page: ink navy, royal blue, ice blue, steel blue, warm gold (on navy only); Source Serif 4 + Source Sans 3
assets/js/main.js              Mobile menu and active nav link
assets/img/                    Headshot, Brandeis photo, social-share image
404.html                       Page shown for broken links
sitemap.xml                    List of all pages, for Google Search Console
.nojekyll                      Tells GitHub Pages to serve the files as they are
```

## Editing content

Homepage content lives in `index.html`; each section has an id (`about`, `research`, `projects`, `publications`, `talks`, `writing`, `contact`). Detail pages live in `research/` and `projects/`.

Content rules from the site's design guide:

- Status labels ("Ongoing Research", "Manuscript in Preparation", …) are not links. Use "Under Review" only once a manuscript is submitted, and "Published" only after publication.
- Only add PDF, DOI, code, demo, slides, Google Scholar or other links once the real destination exists. No placeholder links.
- The resume is always called "Academic Resume", never "Academic CV".
- Writing entries link only to full articles.

When you change `assets/css/style.css`, bump the `?v=` number on its `<link>` in every page so browsers fetch the new styles right away.

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
