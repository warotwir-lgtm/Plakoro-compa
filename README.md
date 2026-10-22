# Plakoro Companion v1.1 beta

Static web app (single index.html, no build step) for tracking HP, move cards and match score in Pokémon Plakoro (30th Anniversary edition).

## What is in 1.1 beta

- Three modes: Best of 1, Best of 3, Best of 3 (team: 3 Pokémon, draft 4 moves each, HP carries over, play until one side has all three knocked out)
- Own HP counter (steps of 10), move cards flip with a 1-turn cooldown and return when another move is used
- Thai move cards where available (121 of 144); English cards for the rest, and wherever the Thai card does not match the English one (currently Electric Rush)

## Known limits

- Altaria, Dragonite and promo cards are still English (no Thai file yet)
- Best of 3 and team rules are house rules, not official rules
- Only your own side is tracked; opponent KOs are entered by hand
- Tested with an automated simulation, not yet on many real devices

## Deploy to Vercel

Option A: Vercel CLI
1. npm i -g vercel
2. cd into this folder
3. vercel (Framework Preset: Other, no build command)
4. vercel --prod

Option B: GitHub
1. Push this folder to a GitHub repo
2. Vercel dashboard > Add New > Project > Import the repo
3. Framework Preset: Other. Leave build command and output directory empty. Deploy.

To update: replace index.html, then run vercel --prod again (or push to GitHub).

## App icon

favicon.ico, icon-192.png, icon-512.png, apple-touch-icon.png (180x180) and manifest.json live in the project root. To use your own icon, replace the PNGs with the same names and sizes and keep the artwork inside the central 80%.

## Credits

Character and move data and English card images: PlakoroDB by u/Jollto (https://github.com/Jollto/PlakoroDB), an unofficial fan translation database. Original contributions there are under CC-BY-NC-4.0.
Thai move cards: phillit28 (page: เต๋าบิน).
Plakoro, Pokémon and all related artwork, names and text belong to their respective owners. This is a non-commercial fan project and is not affiliated with or endorsed by them.
Before sharing the link publicly, ask the owners of the data and the Thai cards for permission.
