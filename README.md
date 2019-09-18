# rime-github-actions

An example to run [rime](https://github.com/icpc-jag/rime) on Github Actions with
 [rime-docker](https://github.com/blue-jam/rime-docker).

There are two jobs in `.github/workflows/test-rime-docker.yml`:

- `test` which runs `rime test`
- `deploy-summary` which generates an HTML with `rime htmlify_full -k` and deploy the page to GitHub Pages on `gh-pages`
branch. [GitHub pages for this project](https://blue-jam.github.io/rime-github-actions/)

The jobs runs on `git push` on the `master` branch.

## Link

- [rime](https://github.com/icpc-jag/rime)
- [rime-docker](https://github.com/blue-jam/rime-docker)
- [peaceiris/actions-gh-pages](https://github.com/peaceiris/actions-gh-pages) - used to publish GitHub pages. You have
to generate & configure `ACTIONS_DEPLOY_KEY`.
