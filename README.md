# Family Caregiver Practical Guide

Static site for [caringforparentsguide.com](https://caringforparentsguide.com/). GitHub Pages deploys the files in this repository from the `main` branch root. There is no build step.

## Preview locally

From the repository root:

```bash
python3 -m http.server 8000
```

Open `http://127.0.0.1:8000/`.

## What is here

- Home page with the five guides, plus one page per guide
- About, Contact, Privacy Policy, and Disclaimer, linked in the header and footer
- `404.html`, `sitemap.xml`, and `robots.txt` for `https://caringforparentsguide.com`
- `CNAME` containing `caringforparentsguide.com`

Internal links are relative, so the same files work at `https://caringforparentsguide.com/` and at `https://m753419-commits.github.io/caringforparentsguide/` while the custom domain is being connected. Canonical URLs use the custom domain. `404.html` uses root-relative links, plus a short script that adds the `/caringforparentsguide/` prefix only on `github.io`, because GitHub serves that file at the missing address.

## Before you publish for readers

1. In `contact/index.html`, replace `[contact email coming soon]` with a real email address and make it a `mailto:` link. That placeholder is the only contact address on the site. The privacy policy and disclaimer point here instead of repeating an address.
2. The guides still say “my book” and name *When You're Caring for a Parent: A Practical Workbook for Adult Children*. That wording is kept from the source articles. The personal byline was not published; the publisher on every page is Family Caregiver Practical Guide. Edit those paragraphs if the workbook mention should not stay.
3. Confirm the domain’s DNS points at GitHub Pages. This repo only sets the `CNAME` file.
4. Advertising code is not included. The privacy policy already says that Google and other third-party vendors may use cookies to serve ads, and it links to [Google’s advertising and cookies policy](https://policies.google.com/technologies/ads).
