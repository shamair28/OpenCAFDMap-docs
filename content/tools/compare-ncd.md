+++
title = "Compare NCD"
weight = 1
+++

Two NCD files side by side, with the same names and value labels as the FDL editor.

- **NCD File 1** / **NCD File 2**: the file pickers open in E-Sys's CAF folder. **Compare** lines both files up
  function by function (group, byte, mask), so two versions of the same CAFD compare too.
- **NCD 1 is on the left and NCD 2 on the right.** Every function whose value differs is red on the right, and both
  sides scroll together. **Differences only** hides the identical rows.
- **Save diff** writes the differences as a tab-separated file (`NCD_diff_<cafd>_<v1>_vs_<v2>.tsv`) that opens in
  Excel or any editor: a `#` header with both files and CAFD versions, then one row per difference (`status`,
  `cafd_id`, `address`, `group`, `function`, `start`, `end`, `mask`, `hex1`, `value1`, `hex2`, `value2`).
- **Without a definition for that CAFD version**, the panel decrypts the CAFD with E-Sys's own PsdZ and builds the
  definition first (a few seconds).
- **Read-only:** Compare NCD never writes an NCD. To change coding, use the FDL editor as usual.
