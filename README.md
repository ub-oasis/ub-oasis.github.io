# OASIS Research Lab Website

This repository hosts the official website for the **Optimizing Artificial Intelligence Solutions and Infrastructure for Science (OASIS) Research Group**, led by Dr. Varun Chandola.

The site is built with Jekyll and powered by the modern [sbryngelson/academic-website-template](https://github.com/sbryngelson/academic-website-template).

---

## Features

- **Searchable Publications**: Powered by `jekyll-scholar`, with live search, downloadable PDFs, DOI links, and BibTeX modals.
- **Dynamic Research Projects**: Categorized cards for active and completed research thrusts with funding agency badges.
- **Lab Team Directory**: PI profile, active postdocs/doctoral researchers, and alumni directory with affiliations and headshots.
- **Modern UI**: Dark/Light mode switcher, frosted glass navbar, responsive typography, and `Cmd+K` site-wide search.
- **GitHub Actions Deployment**: Automatic builds and deployments on push to `main`.

---

## Local Development

### Prerequisites
- Ruby (3.2+ recommended)
- Bundler (`gem install bundler`)

### Setup & Run
```bash
# 1. Clone repository
git clone https://github.com/ubdsgroup/ubdsgroup.github.io.git
cd ubdsgroup.github.io

# 2. Install dependencies
bundle install

# 3. Start local development server
bundle exec jekyll serve --livereload
```
Open [http://localhost:4000/](http://localhost:4000/) in your browser.

---

## Site Content & Editing Guide

- **Site Settings & Identity**: `_config.yml`
- **Publications / Papers**: `assets/ref.bib` (PDFs stored in `papers/`)
- **Research Projects**: `_pages/research.md`
- **Team Members & Alumni**: `_data/team_members.yml` and `_data/alumni.yml` (Photos in `images/team/`)
- **News & Announcements**: `_data/news.yml` and `_pages/news.md`
- **Teaching**: `_pages/teaching.md`
- **About PI & Contact**: `_pages/about.md` and `_data/pi.yml`

---

## License

Source code is available under the MIT License.
Template based on [sbryngelson/academic-website-template](https://github.com/sbryngelson/academic-website-template).
