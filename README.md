# viaEntropia Website

Official website for **viaEntropia** — built with Jekyll and hosted on GitHub Pages.

---

## Overview

This is a lightweight, static one-page website designed to present the band, share information, and provide booking/contact details.

The site is built using:

* Jekyll (static site generator)
* GitHub Pages (hosting & deployment)

---

## Project Structure

```
.
├── _config.yml
├── index.md
├── _layouts/
│   └── default.html
├── _includes/
│   ├── hero.html
│   ├── about.html
│   ├── members.html
│   ├── concerts.html
│   └── contact.html
├── assets/
│   ├── css/
│   │   └── style.css
│   └── images/
```

---

## Editing Content

All content is split into sections for easy editing:

* Hero section → `_includes/hero.html`
* About → `_includes/about.html`
* Members → `_includes/members.html`
* Concerts → `_includes/concerts.html`
* Contact → `_includes/contact.html`

To update the website:

1. Edit the relevant file
2. Commit changes
3. GitHub Pages will automatically rebuild the site

---

## Images

All images should be stored in:

```
/assets/images/
```

Example usage in HTML:

```
<img src="{{ '/assets/images/logo.png' | relative_url }}">
```

---

## Local Development (Codespaces)

If using GitHub Codespaces:

Run:

```
bundle install
bundle exec jekyll serve --host 0.0.0.0 --port 4000
```

Then open the forwarded port (4000) to preview the site.

---

## Deployment

The site is automatically deployed via GitHub Pages.

Settings:

* Source: `main` branch
* Folder: `/root`

After each commit, the site updates automatically.

---

## Custom Domain (optional)

To use a custom domain:

1. Add a `CNAME` file to the repository
2. Configure DNS to point to GitHub Pages
3. Enable HTTPS in repository settings

---

## Notes

* This is a static site — no backend or database
* Contact forms require external services if needed
* Keep images optimized for fast loading

---

## Future Improvements

* Add concert data via `_data/` files
* Improve styling and animations
* Add embedded media (Spotify / YouTube)
* Expand band member profiles

---

## License

All content belongs to viaEntropia.
