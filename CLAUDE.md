# CLAUDE.md — fdmedicis.github.io

<!-- review-gate
visibility: public
-->

My public landing page and portfolio. GitHub Pages serves `main` directly, so
**whatever lands on `main` is live.** There is no deploy step to catch mistakes.

## Rules
- **Public repo: every change goes through a pull request.** Never push to `main`.
- **The cross-model review gate is a required check on pull requests**
  (`.github/workflows/review-gate.yml`). Never remove, skip or weaken it without my
  explicit approval in the pull request.
- **Asymmetric merge.** The required "owner approval" check passes at once for a VALID
  low-risk pull request, and only after my approval of the exact head commit for a
  high-risk one (the files below count as high risk whatever the reviewer says).
  You act as the `ferlab-claude` GitHub App: open the pull request and enable
  auto-merge (`gh pr merge --auto --squash`); low risk then goes live by itself and
  high risk waits for me. Never use my personal credentials to approve or merge.
- **Content is public and professional.** Nothing offensive, misleading or
  infringing. Only images I have the right to publish.
- **No secrets, ever.** No tokens, keys or private contact data beyond what is
  already published on the page.
- **Security files are high risk:** `.well-known/security.txt` and
  `static/files/fdmedicis.pub` (my public PGP key). Do not change them unless I ask.
- Low risk (proceed, the gate still reviews the PR): text, styling, layout, images,
  the CV file. High risk (escalate first): workflows, this file, security files,
  anything touching how the site is served.
- `.github/workflows/deploy.yml` is a manual, optional AWS deploy (S3 + CloudFront).
  It runs only by hand.
