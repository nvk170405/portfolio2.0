# Codex Notes - navketansingh.dev

Static site generator for personal portfolio using Python (Jinja2, Mistune) and Tailwind CSS.

## Working Rules

- Rebuild the preview every time you finish a change before responding.
- After rebuilding, tell the user what to refresh and which page to inspect.
- Edit source files in `src/` and `public/`, not generated files in `dist/`.
- Keep writing natural and understated. Do not make pages feel braggy or corporate.
- On homepage changes, check both desktop and mobile behavior.

## Preferred Rebuild Commands

```bash
uv run python src/build.py --output dist
pnpm tailwindcss -i ./src/index.css -o ./dist/index.css --minify
```

## Dev Server

```bash
pnpm dev
```

## Repo Structure

- `src/build.py` - static site generator
- `src/templates/` - Jinja2 templates
- `src/index.css` - Tailwind source
- `public/` - static assets
- `dist/` - generated output
