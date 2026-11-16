+++
title = "Command line"
weight = 1
+++

Run from the install folder:

```
python ocm\pipeline.py build | names | check     same as OpenLauncher's buttons
python ocm\esys.py launch                         start E-Sys with Open CAFD Map
python ocm\runtime_defs.py --all                  rebuild the definitions E-Sys made on demand
python ocm\defdb.py search 5AC --cafd 000043AF    query the definition DB
python ocm\bc_tool.py show latest:BDC_BODY3 --group 3221
python ocm\cod_import.py --sheet                  BimmerCode backup diffs -> a sheet to name
python ocm\check_names.py --db                    which names match your DB
python ocm\updater.py [--update]                  check for (or install) definition updates
```

The Backup Editor's commands are in [Backup Editor: Command line](@/backup-editor/command-line.md).
