+++
title = "Setup"
weight = 1
+++

1. In OpenLauncher, set **BimmerCode backups** to the folder where you copied BimmerCode's backups from the phone,
   then press **Save settings**.
2. Set the **E-Sys folder**, if you haven't yet. You don't need **Build definitions**.
3. Open **BimmerCode Backup Editor**, then press **Import new backups from source folder**. This copies them into
   `workspace\bimmercode\`:

```
originals\   copies of your backups (never written; "Check originals" verifies them against the source)
decoded\     one .txt (every parameter, name, value, label) + one .json (raw blocks) per backup
edits\       edit files for the command line (EXAMPLE.tsv)
out\         new backups made by the editor (+ a .txt log next to each)
```

## Definitions for your backups
When you open the editor or import backups, it decrypts only the CAFD versions your backups use from your psdzdata
and builds its own definitions from them, with every name that ships with Open CAFD Map. The first time usually
takes under a minute. After that it only runs again for new CAFD versions or when the shipped names update.

- A version your psdzdata doesn't have is listed after the import. Those backups can't be edited until your
  psdzdata has that version.
- Android backups don't store the module's diagnostic address, so the list shows `-` there.
