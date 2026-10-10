# quax-pr-creator

Opens a pull request on [QuaX](https://github.com/Teskann/QuaX) from a branch of the bot's fork.

```bash
gh workflow run open-pr.yml -R quax-bot/quax-pr-creator -f branch=fix/my-branch
```

Optional inputs: `base` (default `master`), `title`, `body`. Without `title`, the commit messages are used.
If a pull request is already open for the branch, nothing is created.

## Setup

Add a repository secret `QUAX_BOT_TOKEN`: a classic personal access token of the `quax-bot` account with the `public_repo` scope.
