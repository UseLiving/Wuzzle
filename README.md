# Wuzzle

Every coin gets a wuzzle: a little AI creature that works for the coin's holders. It posts, keeps the promises its creator sets (buybacks, burns, paydays, milestones), and the rules stop it from doing anything it wasn't allowed to.

## What's in here

- `index.html` — the whole site in one file. Host it anywhere static (GitHub Pages: Settings → Pages → deploy from `main`).
- `assets/wuzzle-logo.svg` — the blue mascot, also used as the favicon.

## What works today

- **Shape a wuzzle:** name, ticker, personality, color, hooks with your own numbers, and per-move / per-day spending caps.
- **Sandbox market:** move the price, add fees and holders, skip days and weeks. Hooks fire on their own, caps trim or block spending, and forbidden requests (send the treasury to the creator, dump the treasury, loosen caps) are refused with the rule that blocked them. Every action leaves a receipt.

## Two modes for the wuzzle's voice

- **Inside a Claude artifact**, the wuzzle's mission, posts and replies are written live by Claude on the viewer's account.
- **Anywhere else** (including GitHub Pages), that isn't available, so the page uses built-in preview lines. To get live AI posts on your own host, replace the `sample` / `sample.json` calls with calls to your own backend.

## Not live

No coin, treasury or chain integration exists. All market numbers are a simulation and are labeled as such. Not financial advice.
