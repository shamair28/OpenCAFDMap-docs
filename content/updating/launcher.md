+++
title = "Launcher updates"
weight = 1
+++

**Update launcher** (under **Updates**) downloads the latest release's `OpenLauncher-Setup.bat` and runs it for the
folder OpenLauncher is installed in, even if that isn't the default folder.

1. Close E-Sys first: it runs Open CAFD Map's files from the install folder.
2. OpenLauncher closes, setup replaces the program files and OpenLauncher starts again. `workspace\` and
   `config.json` are kept.
3. Any edits you made in `names\`, `definitions\` or `data\` are backed up to `workspace\backups\` first.

If the release's definitions are older than the ones you had, OpenLauncher offers the newer definitions again right
after.

Running setup again does the same. A source checkout without a `VERSION` file (not a release install) can't update
itself: install a release, or use a [git clone](@/updating/git-clones.md).
