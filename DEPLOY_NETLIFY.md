# Deploy to Netlify (Next Runtime)

This repo supports both **Vercel** and **Netlify**.

## Netlify settings
- Base directory: (empty)
- Build command: `npm run build`
- Publish directory: **leave empty** OR set to `.netlify/static`
- Plugin: `@netlify/plugin-nextjs` (auto via `netlify.toml`)

## Important
If you previously set Publish directory to `.next` in the Netlify UI, remove that override.
The Next plugin outputs the static assets into `.netlify/static` and wires server rendering via functions.
