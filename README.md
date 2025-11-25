# Hi 👋 I'm brijeshzzzz

> Personalized GitHub metrics dashboard — auto-generated.

![Metrics](https://raw.githubusercontent.com/brijeshzzzz/brijeshzzzz/main/metrics.svg)

---

## How this works

- The GitHub Action `.github/workflows/metrics.yml` runs `lowlighter/metrics` and writes `metrics.svg` into this repository.
- The README embeds `metrics.svg` (the image above), which is automatically updated.

## Setup checklist

1. Create a repository named exactly: `brijeshzzzz` (if not already done).
2. Add the files:
   - `.github/workflows/metrics.yml` (the workflow above)
   - `README.md` (this file)
3. In the profile repo go to **Settings → Secrets and variables → Actions → New repository secret**
   - `Name`: `METRICS_TOKEN`
   - `Value`: your fine-grained personal access token (do **not** paste this anywhere public)
4. (Optional) If you enable PageSpeed or other plugins that need API keys, add the appropriate secret(s) (e.g. `PAGESPEED_KEY`).
5. Trigger the action from **Actions → Generate GitHub Metrics → Run workflow** or wait up to 12 hours for the schedule to run.
6. The workflow will create/update `metrics.svg`. The README will show it automatically.

---

## Tweaks you can make

- Change `plugin_*` options in the workflow to show/hide features (languages, habits, achievements, pagespeed, etc).
- If your default branch is not `main`, update the branch name in the commit step.
- To enable PageSpeed for a specific site, add `PAGESPEED_KEY` as a secret and uncomment the key line in the workflow.
- If you want the action to run more/less frequently, edit the `cron` schedule.

---

If you want, I can:
- add/remove plugins to match the exact screenshot (e.g., 3D contribution graph, PageSpeed circles, suggested tracks),
- or produce a second variant with a different layout (compact / wide).

Tell me which exact widgets from the screenshot you want (or say "exact copy") and I'll update the workflow for that.
