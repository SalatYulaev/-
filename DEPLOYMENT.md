# Luma Jury deployment checklist

## GitHub Pages

1. Open repository Settings → Pages.
2. Under Build and deployment, choose Source = GitHub Actions.
3. Open Actions → Deploy Luma Jury preview.
4. Rerun the latest failed run.
5. Confirm the page loads at https://salatyulaev.github.io/-/.

The current workflow is already committed at .github/workflows/deploy.yml. GitHub's action failed only at Configure Pages because the Pages site is not enabled and the integration cannot create it.

## Important product limitation

The current index.html uses browser localStorage. It is a public click-through preview, not a shared beta. Each visitor sees only their own local tests and votes.

## Before shared beta

- Create independent Supabase project.
- Apply and review supabase-schema.sql from the source package.
- Configure SUPABASE_URL and the public anon/publishable key; never expose service_role.
- Run security checks on RLS and RPC functions.
- Test with two accounts and a second browser/device.
- Set Telegram bot menu URL after HTTPS deployment; add server-side initData verification before claiming Telegram authentication.
- Replace draft privacy details and define the operator, contact, hosting region and retention period.