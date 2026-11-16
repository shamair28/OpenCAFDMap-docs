+++
title = "Definition updates"
weight = 3
+++

New names and definition files are merged into the repository all the time; you don't need to reinstall to get them.
OpenLauncher's definitions button under **Updates**:

- **Check for updates.** Also runs quietly when OpenLauncher opens. The label shows your installed definitions
  version and the latest available one.
- **Update now.**
  1. Downloads the latest `names\`, `definitions\` and `data\` from GitHub and verifies every file against the
     published checksums.
  2. Backs up any of your own edits to those folders (to `workspace\backups\`) and swaps the new files in.
  3. Re-applies names, so E-Sys and the Backup Editor use them straight away.
- **Definitions up to date.** Nothing to do; clicking checks again.

Your workspace (DB, settings, `my_names.tsv`) is never touched. The definitions version (for example `2026.11.13.5`)
is bumped automatically on GitHub after every merged contribution.

Updates only ever come from the Open CAFD Map repository on GitHub, over HTTPS. The source is fixed in the code and
can't be changed in the settings.

Command line: `python ocm\updater.py` checks, `python ocm\updater.py --update` updates.
