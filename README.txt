khuongntrd.github.io
====================

Personal site for Khuong Nguyen, served via GitHub Pages at
https://khuongntrd.github.io. Two parts live in this repo:

1. Portfolio (root) - static HTML/CSS/JS site, served directly from the
   repo root.
2. Blog (/blog)      - Astro site, built from source in blog-src/ and
   committed as static output.

Directory Structure
-------------------
index.html        - Portfolio homepage.
css/               - Stylesheets for the portfolio (main.css is the one to edit).
images/            - Images used by the portfolio.
scripts/           - JavaScript used by the portfolio.
favicon.ico        - Portfolio favicon.
blog-src/          - Astro source for the blog (edit here, not in blog/).
blog/              - Built output of blog-src/, served at /blog. Do not
                     edit by hand; regenerate via `npm run build` in
                     blog-src/ (see blog-src/README.md).
LICENSE-free.txt   - License for the portfolio template (super-folio by
                     TemplateFlip).

Editing the Portfolio
----------------------
1. Content: edit index.html directly, then reload it in a browser to
   check changes.
2. Styles: edit css/main.css.
3. Images: replace files in images/, keeping filenames the same, or
   update the references in index.html if you rename them.

The portfolio is used under TemplateFlip's free license, which requires
keeping the credit link to templateflip.com in the site footer
(see LICENSE-free.txt).

Editing the Blog
-----------------
The blog is an Astro project. Source lives in blog-src/; the built
static site is committed to blog/ and deployed as-is (there is no
build step on the server). See blog-src/README.md for setup, dev
server, and the manual build/commit workflow.

Deployment
----------
This repo is a GitHub Pages user site: whatever is committed to the
repo root (portfolio) and blog/ (blog) is served directly, no CI build
step. After editing the blog, remember to run the Astro build and
commit the regenerated blog/ output along with your blog-src/ changes.
