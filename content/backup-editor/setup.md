+++
title = "Setup"
weight = 1
+++

1. In OpenLauncher, set **BimmerCode backups** to the folder where you copied BimmerCode's backups from the phone,
   then press **Save settings**.
2. Build the definitions, if you haven't yet.
3. Open **BimmerCode Backup Editor**, then press **Import new backups from source folder**. This copies them into
   `workspace\bimmercode\`:

```
originals\   copies of your backups (never written; "Check originals" verifies them against the source)
decoded\     one .txt (every parameter, name, value, label) + one .json (raw blocks) per backup
edits\       edit files for the command line (EXAMPLE.tsv)
out\         new backups made by the editor (+ a .txt log next to each)
```
