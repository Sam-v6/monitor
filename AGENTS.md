# Agent guidance

- Keep this public repository generic. Do not commit credentials, private project names,
  workflow-specific alert rules, or local runtime state. Deployment-specific rules belong
  in the private orchestration repository and are installed under ignored `prometheus/local/`.
- Before pushing, inspect the tracked diff and verify generated local rules remain ignored.
- For this orchestration work, use an isolated `.worktrees/` checkout and a `Sam-v6/` branch.
  Open a pull request, run applicable checks, and merge it into the default branch after review.
  Do not leave completed work in an unmerged PR or push changes directly to the default branch.
