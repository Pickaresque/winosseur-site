# winosseur-site

The one-page site for Winosseur, served by GitHub Pages.

**This repository is generated output. Do not hand-edit `index.html`.**

It is built in the app repository by `scripts/build-site.js`, from:

- copy already ratified for the App Store listing (the promise line, the subtitle, the
  screenshot captions),
- the five screenshot renders, and
- the Straight answers, fetched from the published posts at
  [winosseur.substack.com](https://winosseur.substack.com) by
  `scripts/fetch-straight-answers.js`.

Nothing on the page is composed for it. Every claim is either already public in a post or
already shipped in the app, which is what makes the page sayable at all: a new public product
claim needs a cited path, and a post that already exists is the citation.

When a new Winey Opines post publishes, re-run the fetcher and the builder in the app repo and
copy `docs/site/` here. The page grows; nobody edits HTML.

**`.nojekyll` is load-bearing.** Without it GitHub Pages runs Jekyll, which excludes paths
beginning with an underscore.
