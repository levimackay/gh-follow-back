# gh-follow-back

Follows back anyone who follows levimackay on GitHub and isn't already followed.

Runs on a schedule via GitHub Actions (`.github/workflows/follow-back.yml`), every 6 hours. No local state files — each run diffs the live followers list against the live following list, so there's nothing to drift or get out of sync.

## Setup

1. Create a classic personal access token at https://github.com/settings/tokens with only the `user:follow` scope. Nothing else is needed.
2. In this repo's settings, add it as an Actions secret named `FOLLOW_BACK_TOKEN`.
3. The workflow runs automatically from then on, or trigger it manually from the Actions tab.

**Last updated:** 2026-08-29 11:47 PDT

