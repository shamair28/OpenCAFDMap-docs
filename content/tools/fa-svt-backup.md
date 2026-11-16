+++
title = "FA / SVT auto-backup"
weight = 3
+++

Every FA and SVT that E-Sys reads from the vehicle is saved as a copy in E-Sys's data folder (`Path.Home`, for
example `C:\Data`), with no button to press.

- **FA:** `FA\FABak\<series>_<last 7 of VIN>.xml`; **SVT:** `SVT\SVTBak\<series>_<last 7 of VIN>.xml`. The files are
  E-Sys's own FA / SVT XML, so **Load** opens them like any other.
- **Covered:** Vehicle Order **Read** and SVT Actual **Read (VCM)** / **Read (ECU)** in Coding, and the FA and SVT
  editors. Files you **Load** aren't copied, and neither is the calculated SVT target.
- **Older backups are kept:** if the backup for that car already exists with different content, it's renamed to
  `<name>_<date-time>.xml` first. Reading an unchanged car again doesn't add a copy.
- **Log:** every backup is written to `agent.log`. Tested on E-Sys 25.x; on other versions it's tried too, so check
  the folders after your first read.
