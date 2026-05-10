# ai-docs-test-public

This repository hosts HTML + markdown documents authored with the [`ai-docs` Claude Code plugin](https://github.com/anthropics/claude-code) and served by GitHub Pages.

## Layout

```
decks/<YYYY-MM-DD>/<slug>.{md,html}     # MARP slide decks
reports/<YYYY-MM-DD>/<slug>.{md,html}   # pandoc long-form reports
docs/<YYYY-MM-DD>/<slug>.{md,html}      # general HTML pages
```

Every `.html` ships with a paired `.md` source declared via `<link rel="alternate" type="text/markdown">` so AI tools (and the `read` skill) can fetch the clean markdown without parsing the rendered HTML.

## Live URL

Pages serves files at `https://rulyone.github.io/ai-docs-test-public/<path>`.