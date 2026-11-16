+++
title = "Names and definitions"
weight = 6
sort_by = "weight"
+++

Open CAFD Map combines several sources of names into a **definition** for each CAFD version. Everything shared ships
with OpenLauncher, so a fresh install sees every shared name. Only your private `my_names.tsv` and the cheat sheets
you add yourself stay local.

| Source | Where |
|---|---|
| Your own names | `workspace\my_names.tsv` |
| Community names | `names\*.tsv` |
| BMW names from cheat sheets that can't be shipped | `names\cheatsheet\` |
| Contributed definition XMLs and cheat sheets | `definitions\` |
| BMW's untrimmed names | `definitions\untrimmed\` |
| FP criteria labels, option titles, ECU names, reference vehicles | `data\` |
| Older, unverified names | `names\legacy_*.tsv` |

Your own `my_names.tsv` wins over everything, and the community `names\*.tsv` files win over the other shared
sources. `names\legacy_*.tsv` ranks below everything else, so a verified name replaces a legacy one automatically.

- [Coverage](@/names/coverage/index.md)
- [Build definitions and Apply names](@/names/building.md)
- [Definition updates](@/names/updates.md)
