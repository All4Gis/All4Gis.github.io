# All4Gis — Fran Raga

Personal website of **Fran Raga**, Senior Geospatial Software Engineer.

Live site: [all4gis.github.io](https://all4gis.github.io/)

Built with [Jekyll](https://jekyllrb.com/) and deployed via [GitHub Pages](https://pages.github.com/).

## About

Portfolio site showcasing GIS development work, open-source projects, skills and contact information. Originally based on the [Indigo](https://github.com/sergiokopplin/indigo) Jekyll theme, fully redesigned with a modern layout and updated stack.

## Requirements

- **Ruby 3.3.x** (GitHub Pages currently uses Ruby 3.3.4)
- Bundler

> macOS system Ruby (2.6) is **not supported**. Ruby 4.x is also incompatible with the `github-pages` gem at this time.

### Install Ruby 3.3 (Homebrew)

```bash
brew install ruby@3.3

echo 'export PATH="$(brew --prefix ruby@3.3)/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc

ruby --version   # should show 3.3.x
gem install bundler
```

### Alternative: rbenv

```bash
brew install rbenv ruby-build
rbenv install 3.3.4
cd All4Gis.github.io
rbenv local 3.3.4   # uses .ruby-version
gem install bundler
```

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Open [http://localhost:4000](http://localhost:4000).

Optional flags:

```bash
bundle exec jekyll serve --livereload   # auto-refresh on changes
bundle exec jekyll build                # generate _site/ only
```

## Project structure

| Path | Purpose |
|------|---------|
| `_config.yml` | Site settings, bio, social links, SEO |
| `_data/projects.yml` | Featured projects |
| `_data/skills.yml` | Technology categories |
| `_includes/` | Reusable HTML partials (hero, nav, home sections) |
| `_layouts/` | Page layouts |
| `_sass/` | Stylesheets (Sass) |
| `about.md` | About page content |
| `projects.html` | Projects page |
| `assets/images/` | Profile photo and site images |

## Customization

Edit `_config.yml` to update your name, bio, description and social profiles.

Add or update projects in `_data/projects.yml`:

```yaml
- title: My Project
  description: Short project description.
  url: https://github.com/All4Gis/my-project
  tags: [QGIS, Python]
  featured: true
```

Update skill categories in `_data/skills.yml`.

## Deployment

Push to the `master` branch (or your GitHub Pages source branch). GitHub Pages builds the site automatically using the same `github-pages` gem pinned in the `Gemfile`.

## License

© Fran Raga
