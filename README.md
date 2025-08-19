# Movie Recommendation App (MERN + TMDB)

A fullstack project featuring user auth (JWT), movie discovery via TMDB, favorites, watchlist, and simple reviews. Ready for local dev and deployment (frontend: Netlify/Vercel, backend: Render/Heroku).

## Monorepo Structure
```
backend/  - Node/Express API, MongoDB (Mongoose)
frontend/ - React (Vite) SPA
```

## Quick Start

### 1) Backend
```bash
cd backend
cp .env.example .env
# fill MONGO_URI, TMDB_API_KEY, JWT_SECRET
npm install
npm run dev
```
Default API runs on `http://localhost:5000`.

### 2) Frontend
```bash
cd ../frontend
cp .env.example .env
# set VITE_API_URL=http://localhost:5000
npm install
npm run dev
```

## Deployment Hints
- **Backend**: Push to GitHub → Render (Web Service) → set env vars from `.env`.
- **Frontend**: Netlify/Vercel → set build command `npm run build` and publish `dist/`, env `VITE_API_URL` pointing to backend URL.

## Stretch Ideas
- Social follows, lists sharing, PWA, trailer embeds, improved recommendation algorithm.
