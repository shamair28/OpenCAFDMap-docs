+++
title = "Cheat Sheet"
weight = 2
+++

E-Sys's own FDL Editor on the left, cheat sheets on the right.

- **The editor is E-Sys's real FDL Editor module:** load, edit, save and code exactly as usual. An NCD you opened
  with Coding's **Edit NCD** stays open when you switch to Cheat Sheet.
- **Sources:** the right pane lists every cheat sheet entry for the CAFD that's open, from the shared cheat sheets
  (the community sheets and contributed ones) and the sheets in your **Cheat sheets** folder. Values can be value
  names (`aktiv`), hex (`07`) or byte lists for whole records (`04, 52, 44, ...`).

## Compatibility
Each entry is checked against the open CAFD version:

| Mark | Meaning |
|---|---|
| ✓ compatible | The function is at that group, byte and mask, and the value is one of its values. Values given by name, like `aktiv`, are matched through the labels. |
| ● already set | The open NCD already has that value. |
| ◐ partly compatible | Only some steps fit this version. |
| ✎ custom value | A raw value that isn't one of the function's preset values, for example a modified light record. Its length is checked against the function. |
| ✗ not for this version | The function or value doesn't exist here. |

## Using it
- **Filters:** compatible entries only or all, one sheet or all of them, and a search box. Selecting an entry shows
  its steps: group, BMW function name, byte and mask, current value, target value and the sheet's comment.
- **Go to** selects the function in the FDL tree.
- **Apply** sets the entry's values in the FDL editor through E-Sys's own edit path. A preset value is picked from
  the value list; a custom value is entered in the raw value field (`Werte=`), and E-Sys's parsed result is checked
  byte for byte. Only the NCD open in the editor changes, and E-Sys marks it as modified. Saving and coding stay with
  you. Steps that don't fit are skipped and listed.

**Apply** is held back on E-Sys versions OpenLauncher wasn't tested with; see [E-Sys versions](@/e-sys/versions.md).
