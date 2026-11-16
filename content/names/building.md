+++
title = "Build definitions and Apply names"
weight = 2
+++

## E-Sys doesn't need a build
When E-Sys opens a CAFD that has no definition yet, its definition is built in the background within seconds.
See [How it works](@/e-sys/how-it-works.md).

## Build definitions
Decrypts and indexes all of your psdzdata's CAFDs for the main series into the definition DB in your workspace. It
can take a while. The [BimmerCode Backup Editor](@/backup-editor/_index.md) and the command-line search tools need
it.

By default it exports the newest 3 versions of each CAFD plus the versions in your E-Sys SVT, CAF and NCD folders and
your BimmerCode backups. **Export every CAFD version** in [Settings](@/getting-started/settings.md) exports them all.

## Apply names
After you edit names (`my_names.tsv`, `names\*.tsv`) press **Apply names**. It takes a few seconds and also refreshes
the definitions E-Sys built on demand. Then reopen the CAFD in E-Sys.

## Check contributions
Checks the names and definition XMLs before you contribute them; see
[Before you open a pull request](@/contributing/pull-requests.md).
