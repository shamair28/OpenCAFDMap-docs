+++
title = "Before you open a pull request"
weight = 3
+++

1. Press **Check contributions** in OpenLauncher (or run `python ocm\check_names.py --db`). There must be no errors,
   and your rows should match your DB.
2. **Names and definition files only.** Never commit:
   - psdzdata or decrypted psdzdata files (BMW's own CAFD / FAFP XMLs);
   - your workspace DB;
   - NCDs, BimmerCode backups, FA / FP / SVT files;
   - VINs or anything else from your car.

   `.gitignore` blocks the usual file types and the check rejects psdzdata files and VINs, but please look at your
   diff.
3. Only submit files you have the right to share, and keep their licence notice (many community cheat sheets are
   GPL-3.0).

Don't edit `definitions.json`. After your pull request is merged, GitHub bumps the definitions version automatically,
and everyone gets your names through OpenLauncher's **Check for updates** / **Update now**.
