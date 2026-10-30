# Plakoro Companion v2.0

Static web app (single index.html, no build step) for playing Pokémon Plakoro (30th Anniversary edition): HP counter, move cards with cooldown, match score.

## Modes

- Best of One: one game
- Best of Three: first to 2 wins, same character and 4 moves all match
- Team: 3 characters with drafted moves, HP carries over, play until one side has all three knocked out
- One Device: two players on one phone (split screen, top half rotated), automatic win/loss, weakness hint (+20), Best of One or Best of Three

Other features: first-visit tutorial (? button on the home screen), tap-to-select move cards, vibration on KO (Android), screen stays awake during play where supported.

## Data

- 23 characters and 204 move cards from PlakoroDB, including Exploration Box 2
- Thai move cards for 121 cards (ST01-ST09, EBW01). English cards are used for everything else: Altaria, Dragonite, Exploration Box 2 characters, promo cards, and Electric Rush (the Thai wording differs from the English card)

## Known limits

- Only HP and move cooldown are tracked. The app does not roll dice or calculate damage; the weakness hint only reminds you of +20.
- Team and One Device rules are house rules, not official rules.
- One Device does not support Team mode.
- Tested with automated simulations, not on many real devices.

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
