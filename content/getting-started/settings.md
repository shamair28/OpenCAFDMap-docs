+++
title = "Settings"
weight = 4
+++

Settings are saved to `config.json` next to OpenLauncher. It isn't shared and is kept on every update.

| Setting | Use |
|---|---|
| **E-Sys folder** | The folder that contains `E-Sys.bat`, `jre\` and `lib\`. |
| **psdzdata folder** | Leave empty to use the one E-Sys is set up with. |
| **Main series** | The series to build for, as in the CAFDs' FP info (`G020`, `F030`, `G005`, ...). |
| **Reference vehicle** | Shortens value labels to what matters for that vehicle class (series, market, LCI, engine). |
| **E-Sys UI scale** | For E-Sys started by OpenLauncher: **E-Sys default** keeps E-Sys's own setting; 1, 1.25, 1.5 or 2 sets it. Try **1** if E-Sys's window gets drawn over itself on a scaled display. |
| **E-Sys language** | For E-Sys started by OpenLauncher: **English** or **German**; **E-Sys default** keeps E-Sys's own language. |
| **Workspace** | Where the definition DB, decrypted cache, definitions and logs go. Never shared. |
| **BimmerCode backups** | Your car's exact CAFD versions are always exported, and the Backup Editor can import the backups. |
| **Cheat sheets** | Extra FDL cheat-sheet XMLs you have. The public community sheets are already included. Imported locally only, never shared. |
| **ISTA DiagDocDb** | Optional: a decrypted ISTA database for factory option titles. The line under it shows whether the file can be used: ISTA's own DiagDocDb is encrypted, and only a decrypted copy works. Without one, the option titles that ship with Open CAFD Map are used. |
| **Export every CAFD version** | Exports all versions instead of the newest 3 plus the versions in your E-Sys folders and backups. |
| **Try anyway** | Allows Cheat Sheet **Apply** on E-Sys versions OpenLauncher wasn't tested with. |

E-Sys UI scale and language only apply to E-Sys started by OpenLauncher; E-Sys's own settings (`config\Esys.properties`) aren't changed. If the language picked here differs from E-Sys's own, a few texts E-Sys builds later through PsdZ (for example in a TAL) might still come out in E-Sys's own language.
