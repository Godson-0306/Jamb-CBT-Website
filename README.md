# JAMB CBT

This project is now a simple CBT website only.

There is:

- no database
- no admin panel
- no Docker
- no Prisma
- no backend API apart from a tiny local file server

## Run

1. Open a terminal in this folder
2. Run:
   `npm start`
3. Open:
   `http://localhost:3000`

## Main files

- `index.html` - app structure
- `styles.css` - styling
- `app.js` - CBT logic and randomized questions
- `local-server.js` - lightweight local preview server

## Deploy To Vercel

This project should be deployed on Vercel as a static site.

### Why

- `index.html`, `styles.css`, and `app.js` contain the full app
- there is no database or backend dependency for production
- `local-server.js` is only for local preview

### Vercel setup

1. Push this repo to GitHub
2. Import the repo into Vercel
3. Use these project settings if Vercel asks:
   - Framework Preset: `Other`
   - Build Command: leave empty
   - Output Directory: leave empty
4. Deploy

Vercel will serve the root static files directly, with `/` mapped to `index.html`.

### Local preview

Run:
`npm run dev`

Then open:
`http://localhost:3000`
