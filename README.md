# Plakoro Companion

Static web app (single index.html, no build step) for tracking HP, turns and move cards in Pokémon Plakoro (30th Anniversary edition).

## Deploy to Vercel

Option A: Vercel CLI
1. npm i -g vercel
2. cd plakoro-vercel
3. vercel        (answer the prompts; Framework Preset: Other, no build command)
4. vercel --prod

Option B: GitHub
1. Push this folder to a GitHub repo
2. Vercel dashboard > Add New > Project > Import the repo
3. Framework Preset: Other. Leave build command and output directory empty. Deploy.

## Credits

Character and move data and card images come from PlakoroDB by u/Jollto (https://github.com/Jollto/PlakoroDB), an unofficial fan translation database. Original contributions there are under CC-BY-NC-4.0.
Plakoro, Pokémon and all related artwork, names and text belong to their respective owners. This is a non-commercial fan project and is not affiliated with or endorsed by them.
