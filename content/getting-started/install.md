+++
title = "Install"
weight = 2
+++

1. On the [Releases](https://github.com/shamair28/OpenCAFDMap/releases/latest) page, download
   **`OpenLauncher-Setup.bat`** and double-click it. Windows may warn about a downloaded file: choose
   *More info* → *Run anyway* if you trust it.
2. Setup:
   - asks for an install folder (default `%LOCALAPPDATA%\OpenCAFDMap`; no admin rights needed);
   - checks for Python and offers to install it with `winget` if it's missing;
   - downloads the latest release, verifies its SHA-256 checksum and installs it;
   - creates **OpenLauncher** shortcuts on your Desktop and in the Start menu.

## Upgrading
Use **Update launcher** in OpenLauncher, or run setup again. Your `workspace\` folder and settings are kept.
See [Updating OpenLauncher](@/updating/_index.md).

## Manual install
Extract `OpenCAFDMap.zip` from the release (or clone the repository) anywhere and double-click `OpenLauncher.bat`.
OpenLauncher's **Desktop shortcut** button adds a shortcut with the icon.

## Uninstall
Delete the install folder and the OpenLauncher shortcuts.

## Unattended setup
Setup reads these optional environment variables:

| Variable | Use |
|---|---|
| `OCM_SETUP_DIR` | Install folder (default `%LOCALAPPDATA%\OpenCAFDMap`) |
| `OCM_SETUP_ZIP` | Install from a downloaded `OpenCAFDMap.zip` instead of GitHub |
| `OCM_SETUP_TAG` | Install that release (for example the v3 release candidate, `v3.0.0-rc.1`) instead of the latest |
| `OCM_SETUP_QUIET=1` | No questions (Python isn't installed automatically in this mode) |
| `OCM_SETUP_NO_SHORTCUTS=1` | Don't create shortcuts |
| `OCM_SETUP_NO_LAUNCH=1` | Don't start OpenLauncher at the end |
