# semantic-thinking

Structured reasoning applied to the most contested ideas in AI, DPI, fintech, and public discourse. Each post runs a claim or controversy through analytical recipes — assumption audits, first-principles decomposition, inversion, analogy transfer, ladder-of-abstraction mapping, and Nietzschean critique.

## Repository Structure

| Path | Description |
|------|-------------|
| `_posts/` | Jekyll blog posts (markdown, Jekyll front-matter) |
| `_layouts/` | Jekyll layout templates (default, page, post) |
| `images/` | Diagram assets (D2-generated PNGs) |
| `index.html` | Blog home/landing page |
| `about.md` | About page |
| `feed.xml` | RSS feed template |
| `404.md` | 404 page |
| `_config.yml` | Jekyll configuration |
| `Gemfile` | Ruby dependencies (GitHub Pages) |

## Conventions

- **Theme**: Type Theme for Jekyll (light/dark mode via `prefers-color-scheme`)
- **Diagrams**: Generated with D2, exported as PNG to `images/`
- **Diagrams referenced in posts** use absolute paths: `/semantic-thinking/images/<file>.png`
- **Image assets**: Keep PNG file sizes optimized for the web (aim < 500 KB per diagram, use pngquant if needed)

## Deployment

GitHub Pages publishes `master` branch to https://logicinczo.github.io/semantic-thinking/.

## Setup

```bash
bundle install
bundle exec jekyll serve  # local dev at http://localhost:4000/semantic-thinking/
```

### Image generation (D2)

```bash
# To regenerate a diagram from source if .d2 files exist in images/
d2 images/input.d2 images/output.png --theme=200 --layout=elk
```

## Content Guidelines

1. **Claim → Recipe**: Each post starts with a specific claim or phenomenon and applies a structural reasoning recipe from the semantic-algos toolkit.
2. **Image-first**: Complex arguments include a D2-generated diagram as the cognitive anchor before prose.
3. **Evidence density**: Every non-obvious claim has a hyperlinked citation (preferably primary sources).
4. **Tone**: Analytic, precise, non-polemical even when the subject is contested. No outrage, no clickbait.

## Related

- **semantic-algos skill**: `file 'Skills/semantic-algos'` — recipe framework used to structure posts
- **AgriStack research**: `file 'Projects/AgriStack'` — empirical grounding for DPI claims