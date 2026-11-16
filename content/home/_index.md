+++
title = "Home"
weight = 1
sort_by = "weight"
+++

**Open CAFD Map** is an open-source project that maps BMW's coding data back to readable names. **OpenLauncher** is
its free, non-invasive launcher for modern versions of E-Sys: it brings those names into E-Sys without changing
anything in your E-Sys install. The database has been brought up to date to cover most G- and F-chassis coding
definitions and parameters, along with FA / VO option codes.

It also adds a few quality-of-life features, all accessible from inside E-Sys:

- **Compare NCD**: two NCDs side by side, with the differences highlighted
- **Cheat Sheet**: cheat sheets right next to the FDL editor
- **FA / VO and SVT auto-backup**: every FA and SVT you read from the car is saved automatically
- **[FA Helper](@/tools/fa-helper/index.md)** (v3 preview): edit the vehicle order with every option checked against
  the type key, conflicts and the CAFDs your psdzdata has

Where the database falls short, names and parameters are dynamically calculated to fill in the gaps.

<div style="border-left: 4px solid #2e9e5b; background: #13261b; padding: 12px 16px; margin: 1.2em 0; border-radius: 0 4px 4px 0;">
<strong style="color: #4fd18a;">Compatibility</strong><br>
Tested with <strong>E-Sys 25.10</strong> and <strong>E-Sys 3.35.3</strong> on Windows, with Python 3.10 or newer.
It <strong>should</strong> work on all Java 8 and Java 11 builds of E-Sys (<a href="../e-sys/versions/">check the version list</a>),
but universal compatibility hasn't been guaranteed yet.
</div>

![OpenLauncher v2.3.4: paths, definitions, tools, folders and updates in one window](openlauncher-v2.3.4.png)

*OpenLauncher v2.3.4 (current release)*

![OpenLauncher v3.0.0-beta.1: dark theme with a sidebar, the Launch card, status cards, Definitions and Updates](openlauncher-v3.0.0-beta.1.png)

*OpenLauncher v3.0.0-beta.1 ([preview](@/updating/v3-preview.md))*

## Who it's for

OpenLauncher is for people who code with E-Sys and want it to show BMW's real names wherever they exist, plus an
essential set of quality-of-life tools, free and unlocked.

If you want one-click coding presets, guided fault-code help or service resets, paid suites are built for that.
OpenLauncher doesn't try to be one.

## Built to stay out of the way

- **Layout-verified names:** BMW's names are only applied where a function's exact byte layout matches, so they never
  land on bits that moved between software versions.
- **Read-only renaming:** names are changed in E-Sys's tree in memory only. Nothing is patched into E-Sys, and the
  renaming never changes coding data or anything E-Sys sends to the car.
- **Versioned FA / SVT backups:** every FA and SVT read from the car is saved, and older copies are kept rather than
  overwritten.
- **Open and unlocked:** open source (MIT code, CC0 names). Everything runs on your PC, with no account, activation or
  hardware lock. Updates are optional.

[Download OpenLauncher](https://github.com/shamair28/OpenCAFDMap/releases/latest) ·
[Getting started](@/getting-started/_index.md) ·
[GitHub](https://github.com/shamair28/OpenCAFDMap)

OpenLauncher is free. If someone sold it to you, ask for your money back and grab it from GitHub.

Not affiliated with BMW. Your psdzdata and coding data stay on your PC. Code at your own risk.
