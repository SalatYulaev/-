# Luma Jury — Inside Luma

**Не гадай. Проверь на людях.**

This repository contains the first public preview of Luma Jury, a blind A/B feedback room for ideas, names, offers and product framing.

## Current published state

- The current public page is a LOCAL-ONLY DEMO. Tests and votes are stored in the visitor's browser localStorage and are not shared between visitors.
- No real market research, cross-user voting, real accounts, payment, rewards or Telegram bot authentication are active yet.
- Do not use this preview for sensitive or confidential concepts.

## Next release gate

1. Connect an independent Supabase project and apply the reviewed SQL schema with row-level security.
2. Test create, vote from a second account, creator results, duplicate-vote rejection and self-vote rejection.
3. Add verified Telegram Mini App authentication with server-side initData validation and a bot token stored only as a server secret.
4. Review operator identity, privacy notice, data region, retention and moderation contact before opening wider access.

## Deployment

The static preview is deployed through GitHub Actions and GitHub Pages. The workflow uploads the repository root without a build step.

## Scope decision

Luma Jury is a human-feedback product, not a prediction market: no bets, trading, crypto, cash rewards or token economy.