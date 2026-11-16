+++
title = "Git clones"
weight = 2
+++

A git clone follows `origin/main` instead of releases (or `origin/testing` while it runs the
[v3 preview](@/updating/v3-preview.md)). Git must be on `PATH`.

- **Update launcher** runs `git pull --ff-only`, then restarts OpenLauncher.
- **Force update** also works when a plain pull can't run (local edits or commits). It first saves everything, then
  moves the branch to its origin:
  - uncommitted changes go to a git stash (`git stash list`);
  - local commits get a branch named `openlauncher-backup-<time>`.

`workspace\` and `config.json` are git-ignored, so git never touches them. Definition updates in a clone also use
`git pull --ff-only`.
