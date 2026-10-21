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
