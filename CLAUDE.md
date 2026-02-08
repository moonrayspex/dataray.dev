# CLAUDE.md

## Project Overview

Personal portfolio and blog site for dataray.dev, built with Jekyll and deployed to GitHub Pages.

## Tech Stack

- **Framework:** Jekyll 4.3
- **Theme:** Minima 2.5
- **Language:** Ruby
- **Deployment:** GitHub Pages via GitHub Actions
- **Content:** Markdown

## Commands

```bash
# Install dependencies
bundle install

# Run local development server (http://localhost:4000)
bundle exec jekyll serve

# Build for production
JEKYLL_ENV=production bundle exec jekyll build
```

## Project Structure

```
_config.yml        # Jekyll site configuration
_layouts/          # Custom HTML layouts
_posts/            # Blog posts (YYYY-MM-DD-title.md format)
index.md           # Homepage content
about.md           # About page
Gemfile            # Ruby dependencies
.github/workflows/ # GitHub Actions CI/CD
```

## Conventions

- Blog posts go in `_posts/` using the naming format `YYYY-MM-DD-post-title.md`
- All content files use YAML front matter (layout, title, date, etc.)
- Custom layouts go in `_layouts/`
- The site uses Minima theme defaults; only override layouts when customization is needed
- Git workflow uses feature branches and pull requests merged to `main`

## Plugins

- `jekyll-feed` - RSS feed generation
- `jekyll-seo-tag` - SEO meta tags
- `jekyll-sitemap` - Sitemap generation

## Build Output

- Generated site goes to `_site/` (gitignored)
- Cache directories `.jekyll-cache/` and `.sass-cache/` are gitignored
- `Gemfile.lock` is gitignored
