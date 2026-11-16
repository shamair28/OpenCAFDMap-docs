+++
title = "Folder layout"
weight = 2
+++

```
OpenLauncher.bat           OpenLauncher (openlauncher.py)
Start-ESys-OpenCAFDMap.bat E-Sys with names, using the saved settings
names\                     community names (CC0)          <- contributions go here
  cheatsheet\              BMW names from a cheat sheet that can't be shipped
definitions\               contributed definition XMLs and cheat sheets   <- and here
  community-cheatsheets\   public community cheat sheets (GPL-3.0, unchanged)
  untrimmed\               BMW's untrimmed names, by CAFD id
definitions.json           definitions version + checksums (bumped by GitHub; used by the updater)
data\                      FP criteria labels, SA option titles, ECU names, reference vehicles (contexts)
esys\                      scripts that run inside E-Sys started by OpenLauncher
ocm\                       Python tools
docs\                      Backup Editor guide, examples
assets\                    OpenLauncher icon
workspace\                 (created locally, never shared) DB, decrypted cache, definitions, runtime_cafd, logs, backups
config.json                (created locally) your settings
```
