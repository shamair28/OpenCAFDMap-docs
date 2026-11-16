+++
title = "Finding names"
weight = 2
+++

- **BimmerCode backup diffs.** Take a backup, change one option in BimmerCode, take another backup, then run:

  ```
  python ocm\cod_import.py --sheet
  ```

  It lists exactly which parameter changed. Write the BimmerCode option name into the sheet, run
  `python ocm\cod_import.py --apply` (it goes into your private `workspace\my_names.tsv`), then press
  **Apply names**.
- **Screenshots and tables** of tools that still show names, with their source.
- **Your own testing.** Comment-only rows are welcome.

Move rows you're confident about from `my_names.tsv` into the right `names\<ECU>.tsv` (create the file if the ECU has
none yet) and open a pull request.
