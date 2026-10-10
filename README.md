# quax-pr-creator

Opens a pull request on [QuaX](https://github.com/Teskann/QuaX) from a branch of the bot's fork.

```bash
gh workflow run open-pr.yml -R quax-bot/quax-pr-creator \
  -f branch=fix/my-branch -f title="My title" -f body="My description"
```

Required inputs: `branch`, `title`, `body`. Optional: `base` (default `master`).
If a pull request is already open for the branch, nothing is created.

## Setup

Add a repository secret `QUAX_BOT_TOKEN`: a classic personal access token of the `quax-bot` account with the `public_repo` scope.
