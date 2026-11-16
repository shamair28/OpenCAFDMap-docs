+++
title = "Logs and troubleshooting"
weight = 4
+++

Logs are in `workspace\logs\` (OpenLauncher's **Logs** button opens the folder):

| File | Contents |
|---|---|
| `esys.log` | E-Sys's own output for the latest start (the previous one is `esys.prev.log`). Attach it to bug reports. |
| `agent.log` | Names and the tools inside E-Sys |
| `runtime_defs.log` | Definitions built on demand when you open a CAFD |
| `decrypt.log` | **Build definitions** |

If E-Sys fails while starting, it closes instead of leaving the splash screen up, and OpenLauncher shows the reason
with the last lines of `esys.log`.

## Ruling out OpenLauncher
In the [v3 preview](@/updating/v3-preview.md), **Launch options → Clean boot** starts your `E-Sys.bat` exactly as it
is, with none of OpenLauncher's features. If E-Sys misbehaves there too, the problem isn't OpenLauncher.

Problems and questions: [open an issue](https://github.com/shamair28/OpenCAFDMap/issues) and attach `esys.log`.
