# Family Caregiver Practical Guide

Static site for [caringforparentsguide.com](https://caringforparentsguide.com/). GitHub Pages deploys the files in this repository from the `main` branch root. There is no build step.

## Preview locally

From the repository root:

```bash
python3 -m http.server 8000
```

Open `http://127.0.0.1:8000/`.

## What is here

- Home page with all of the guides, plus one page per guide
- About, Contact, Privacy Policy, and Disclaimer, linked in the header and footer
- `404.html`, `sitemap.xml`, `robots.txt`, and `ads.txt` for `https://caringforparentsguide.com`
- `CNAME` containing `caringforparentsguide.com`

Internal links are relative, so the same files work at `https://caringforparentsguide.com/` and at `https://m753419-commits.github.io/caringforparentsguide/` while the custom domain is being connected. Canonical URLs use the custom domain. `404.html` uses root-relative links, plus a short script that adds the `/caringforparentsguide/` prefix only on `github.io`, because GitHub serves that file at the missing address.

## Before you publish for readers

1. The site intentionally shows no email address or contact form. `contact/index.html` says so, and the privacy policy and Medicare corrections page point to it. Do not add an address unless the owner asks for one.
2. Every guide and Medicare page is published under the organization name Family Caregiver Practical Guide (visible byline, `meta name="author"`, and JSON-LD `author` and `publisher`). No page presents a personal author or a personal caregiving story. The KDP books are still listed as books by Ellen Carter in the “Books by Ellen Carter” sections; that is the books' own byline, not a claim about who writes this site.
3. Confirm the domain’s DNS points at GitHub Pages. This repo only sets the `CNAME` file.
4. Google AdSense site verification is present: `ads.txt` and a `google-adsense-account` meta tag on every HTML page. The AdSense script and ad units are not included. The privacy policy already says that Google and other third-party vendors may use cookies to serve ads, and it links to [Google’s advertising and cookies policy](https://policies.google.com/technologies/ads).
