+++
title = "E-Sys versions"
weight = 3
+++

| E-Sys | Java | Status |
|---|---|---|
| 25.10 | 11 | Tested: names, on-demand definitions, Compare NCD, Cheat Sheet, FA / SVT backup, FA Helper (v3 preview) |
| 3.35.3 | 8 | Tested: names and on-demand definitions. The OpenLauncher section needs E-Sys 25.x's navigation bar. |
| Java 15 or newer | | Can't be started this way (Java's JavaScript runner was removed). OpenLauncher says so. |

**Other E-Sys versions** (for example 22-24 or 26) are tried rather than blocked. Names, Compare NCD, the Cheat Sheet
window and the FA / SVT backup run wherever E-Sys has what they need, and switch themselves off (with a line in
`agent.log`) where it doesn't. Only Cheat Sheet **Apply**, which edits through E-Sys's FDL Editor, is held back on
versions OpenLauncher wasn't tested with: tick **Try anyway** in OpenLauncher's settings to allow it there.
