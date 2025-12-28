# PAY402WIN Lottery (Solana)

A simple on-chain-payment **lottery-style** web app on **Solana mainnet**.

**Live:** https://pay402win.com

![PAY402WIN preview](./public/images/preview.png)

## What this is

A lightweight demo that lets a user:

1. Pick a number **1–402**
2. Pay **0.003 SOL** from their wallet
3. Win and claim your payout 🏆

> Note: the current “result” / spin logic is client-side demo logic. If you need provably-fair outcomes, add an on-chain program + VRF oracle / backend verification.

## Payment

- **Cost per play:** 0.003 SOL


## Tech stack

- Next.js (App Router) + React
- Tailwind + shadcn/ui
- Solana Wallet Adapter + `@solana/web3.js`
- `sonner` for toasts

## Local development

```bash
pnpm install
pnpm dev
```

Open http://localhost:3000

### Optional env

Create `.env.local` (optional):

```bash
# Custom RPC (otherwise uses clusterApiUrl("mainnet-beta"))
NEXT_PUBLIC_SOLANA_RPC_URL=
```

## Deploy

Recommended: **Vercel** (import the repo, set env vars if needed, deploy).

## Phantom warning on new domains

Phantom may show a security interstitial on **new / low-reputation** domains (“This dApp could be malicious…”).
That warning is controlled by Phantom. If you own the dApp, submit the domain for review via Phantom support
(the wallet prompt includes the contact email).

## License

MIT
