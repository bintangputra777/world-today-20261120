# Dossier — make.fun bounty "Sum up 20 November's world news in one image"

## Bounty (verified 21 Nov 2026, ~08:45 WIB)

- Bounty: **Sum up 20 November's world news in one image** — https://make.fun/bounty/news-image-20261120
- Slug: `news-image-20261120` · Prize: **$250, 50 places paid** (1st $50, 2nd $30, 3rd $15, 4th–10th $5 each, 11th–50th $3 each), USDC on Solana, escrow funded 2026-11-20.
- Deadline: **Sunday 22 Nov 2026, 07:00 WIB** (2026-11-22T00:00:00Z).
- Judging: an AI judge that can see images compares entries two at a time; the image itself must show the day's news (the judge has no news feed).
- Same format as the accepted 19 Nov entry (world-today-20261119); this build reuses its verified render pipeline.

## The image — five stories (checked 21 Nov against OneTurn, Open Chronicle, Just Security, Bangladesh Chronicle, all dated 20 Nov 2026)

1. **JUSTICE — World Court: Myanmar committed genocide.** The ICJ finds Myanmar's forces committed genocide against the Rohingya — first such finding against a state by that court, decided 9–6. (On 19 Nov the ruling was still pending; it landed on the 20th.)
2. **SUMMIT — Trump, Xi & Putin sign peace declaration.** Four-point joint declaration after the first three-way Shenzhen meeting.
3. **MARKETS — AI sell-off rocks global stock markets.** AI-valuation doubts after Anthropic's Nasdaq debut: Nikkei −4.8%, S&P 500 down a fifth straight day.
4. **RIYADH — Houthi missiles hit Riyadh finance district.** The sovereign wealth fund (PIF) tower damaged; Saudi defences intercepted more missiles/drones.
5. **UKRAINE — Russia pounds Kyiv in missile barrage.** Bridges and districts hit, eight killed; Ukraine replied with drones on a chemical plant in Russia's Smolensk region.

Design: same newspaper front-page style as the 19 Nov entry — navy masthead "THE WORLD TODAY / FRIDAY · 20 NOVEMBER 2026", five numbered colour-tagged rows, footer citing major news outlets. Rendered in code with Python/PIL (`scripts/render.py`) — no AI image generator.

## Program

`main.ts` copies `assets/entry.png` to `/output/entry.png` — deterministic, no network. Verified locally: two runs byte-identical and equal to the source asset.
