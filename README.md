# Dubbing QC — site

Static landing page + privacy policy for Dubbing QC. No build step, no
dependencies — one stylesheet, two HTML files, local images only.

Built ahead of domain registration: there's no `CNAME` file yet and the Open
Graph / canonical URLs in `index.html` and `privacy.html` point at local
files, not a live domain. Once a domain is registered:

1. Add a `CNAME` file with the domain (one line, no protocol).
2. Fill in `<link rel="canonical">`, `og:url` and `og:image`/`twitter:image`
   absolute URLs in both HTML files.
3. Point the domain's DNS at GitHub Pages (four `A` records to
   `185.199.108–111.153`, or a `CNAME` record to `jirivatka.github.io` for a
   subdomain).
4. Enable the custom domain in the repo's Settings → Pages.

Until then the site is live at the default `github.io` Pages URL.

Content stays in step with `docs/Manual.html` and `docs/DubbingQC.md` in the
app's own repo — the check list and export formats here should match what's
actually shipped.
