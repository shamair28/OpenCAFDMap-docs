+++
title = "v3 preview"
weight = 3
+++

OpenLauncher v3 is in preview: a new dark design, **Launch options** and the [FA Helper](@/tools/fa-helper/index.md). It's published as a GitHub
[pre-release](https://github.com/shamair28/OpenCAFDMap/releases), so normal updates and setup keep installing the
stable release until you choose to try it.

## Try it
In OpenLauncher 2.3.4 or newer: **Updates → Try OpenLauncher v3**.

- **Release install:** installs the newest v3 pre-release into the same folder. Your workspace and settings are kept,
  and edited name files are backed up first.
- **Git clone:** switches the clone to the `testing` branch. Uncommitted changes go to a git stash and local commits
  to a backup branch first.

While you're on the preview, **Update launcher** offers newer previews, and the final v3 release once it's out.

## Go back
In v3: **Updates → Back to stable**. It installs the latest stable release (or switches a git clone back to `main`).
Your workspace is kept. Launch options are reset to their defaults (everything on) once v2 saves its settings.

## Launch options
Under **Start E-Sys**, **Launch options** chooses what E-Sys gets when OpenLauncher starts it. Changes apply from the
next E-Sys start.

| Option | What it does |
|---|---|
| **Name Injection** | Names and value labels in the CAF / FDL trees and the vehicle profile |
| **Build labels on demand** | New CAFD versions are labelled in the background (needs Name Injection) |
| **Additional Utilities** | Compare NCD, Cheat Sheet and FA Helper in E-Sys's navigation bar |
| **FA / SVT auto-backup** | Copies every FA / SVT read from the car to `FA\FABak` and `SVT\SVTBak` |
| **Clean boot** | Troubleshooting: starts your `E-Sys.bat` exactly as it is, with none of OpenLauncher's features |

**Turn all features on** resets them.

## Without OpenLauncher
Download `OpenLauncher-Setup.bat` from the latest stable release and run it with the environment variable
`OCM_SETUP_TAG` set to the preview's tag (for example `v3.0.0-beta.1`). See [Install](@/getting-started/install.md).
