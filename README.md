# PinkFlip — Live Item Coinflips

Clean pink + grey/black coinflip site for Roblox items (MM2-style).

## Features

- Live coinflips (create / join)
- Wallet with inventory + total value
- Deposit flow via bots
- Online bots:
  - **xxcyberl303** → https://www.roblox.com/gg
  - **Silenxit6653** → https://www.roblox.com/fun
- Withdrawals disabled (Coming Soon)
- Discord webhook ready (uses the trade-complete logger)

## Deploy to Vercel

1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com) → New Project → Import the repo
3. Framework Preset: **Other** (static)
4. Deploy — done

Or with CLI:

```bash
npm i -g vercel
vercel
```

## Local preview

Just open `index.html` in a browser, or:

```bash
npx serve .
```

## Webhook integration

The MM2 logger script posts completed trades to Discord.  
Bridge that embed (username + items) to this site to credit wallets.

Currently the site uses localStorage + a "Simulate Deposit" button for demo purposes.

## Notes

- Pure static HTML/CSS/JS — no build step required
- State persists in the browser via localStorage
- For real multi-user live flips add a backend (Supabase / Firebase / custom API + WebSockets)
