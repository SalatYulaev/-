# Luma Jury — Inside Luma

**Не гадай. Проверь на людях.**

Luma Jury is a blind two-option feedback room for ideas, names, offers and product framing.

## Current published state

- The current page is a LOCAL-ONLY DEMO. Tests and votes are stored in each visitor's browser localStorage and are not shared between visitors.
- It does not yet provide real cross-user voting, accounts, live research, payments, rewards or Telegram bot authentication.
- Do not submit confidential or sensitive concepts in this preview.

## Deployment

Repository: https://github.com/SalatYulaev/-

One-time owner action required: open https://github.com/SalatYulaev/-/settings/pages, go to Build and deployment, and set Source to GitHub Actions. The GitHub Actions connection cannot create the Pages site with its current permissions. After enabling Pages, open the Actions tab and rerun the latest 'Deploy Luma Jury preview' run.

Expected URL after successful deployment: https://salatyulaev.github.io/-/

## Next release gate

1. Connect an independent Supabase project and apply the reviewed SQL schema with row-level security.
2. Test create → vote from a second account → creator results → duplicate-vote and self-vote rejection.
3. Add server-side Telegram initData validation with a bot token stored only as a server secret.
4. Review operator identity, privacy notice, data region, retention and moderation contact before opening wider access.

## Product boundary

Luma Jury is a human-feedback product, not a prediction market. No bets, trading, crypto, cash rewards or token economy.

## Files

- index.html — current one-file local-only preview.
- privacy.html — privacy draft; requires operator details and legal review.
- rules.html — beta rules.