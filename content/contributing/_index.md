+++
title = "Contributing"
weight = 8
sort_by = "weight"
+++

The names are the heart of the project, and every name helps everyone with that ECU. There are three ways to
contribute:

- **A few lines in a `names\<ECU>.tsv` file.** Best for names you found yourself, or to fix or fill in anything the
  untrimmed names lack. See [The names format](@/contributing/names-format.md).
- **Untrimmed dumps.** If you have untrimmed CAFD definitions (XML with every function), run
  `python ocm\untrimmed.py pack-dumps <folder>`. It merges them into `definitions\untrimmed\<CAFD id>.tsv.gz` by
  layout and never removes existing names. Open a pull request with the changed `.tsv.gz` files.
- **Whole files in `definitions\`:** definition XMLs (`<CafdDefinition>`) or FDL cheat sheets (`<FDL>`) you already
  have. Their names are merged automatically, and a definition XML also covers people whose psdzdata lacks that CAFD
  version.

Bug fixes and improvements to the code are welcome too. Keep the launcher-only rule: nothing may be installed into,
patched into or written to the E-Sys folder.

- [The names format](@/contributing/names-format.md)
- [Finding names](@/contributing/finding-names.md)
- [Before you open a pull request](@/contributing/pull-requests.md)
