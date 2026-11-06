# Contributing to Campus Hand

1. Branch from `development`: `feature/<slug>`, `fix/<slug>` or `chore/<slug>`.
2. Commit with Conventional Commits (`feat(catalogue): ...`). Commitlint enforces it.
3. Open a PR into `development`. CI must be green. Squash-merge.
4. Releases: PR `development` -> `main`, merge commit (never squash). Backend before frontend.
5. Urgent production fix: `hotfix/<slug>` from `main`, PR into `main`, then PR `main` -> `development`.
6. Never commit secrets. `.env*` files stay local; values live in Render, Vercel and GitHub secrets.
