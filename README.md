# PokeBite — Food Around Me

A single-page, monster-catching-adventure-styled food directory for spots within 2 km of Parc Clematis, Clementi, Singapore. Pure HTML/CSS/JavaScript, no build step, no dependencies.

## Deploy on Vercel (via GitHub)

1. Push this folder to a new GitHub repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: PokeBite"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   git push -u origin main
   ```
2. Go to https://vercel.com/new and import that GitHub repository.
3. Framework preset: choose **Other** (or leave it on "No Framework"). No build command or output directory is needed — `index.html` is served as-is from the project root.
4. Click **Deploy**. Vercel will give you a live URL in about a minute.

Any future push to the `main` branch will auto-redeploy.

## Notes

- This app currently uses labeled **demo data** for restaurants (ratings, hours, delivery links, etc. are placeholders where marked). See the comments in `index.html` (search for "RESTAURANT DATA SOURCE") for where to plug in a real Google Places, Google Maps, or OpenStreetMap/Overpass API.
- Favourites and "discovered" progress are stored in the visitor's own browser via `localStorage` — nothing is sent to a server.
- No API keys are required or embedded for the current demo build.
