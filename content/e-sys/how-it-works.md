+++
title = "How it works"
weight = 2
+++

Open CAFD Map **only runs inside an E-Sys it starts itself**: OpenLauncher's **Start E-Sys** button, or
`Start-ESys-OpenCAFDMap.bat`.

- It starts a **new** E-Sys process from E-Sys's own JRE, classpath and VM options, read from your E-Sys version's
  own `E-Sys.bat`. Only the classpath, working folder, `-X` / `-D` options and main class are taken; other additions
  such as `-javaagent` are left out. Java's built-in JavaScript runner is the entry point: `esys/bootstrap.js` loads
  `esys/agent.js`, then calls E-Sys's normal main class.
- **Nothing is installed into E-Sys**: no edited `.bat`, jar, config file, `-javaagent` hook or environment variable.
  The E-Sys folder is only read. E-Sys started any other way (`E-Sys.exe`, `E-Sys.bat`, another launcher) never sees
  Open CAFD Map's code.
- Both scripts **refuse to run** unless OpenLauncher's `-Docm.launcher=1` switch is present.
- The agent only **renames tree nodes in memory**. It never changes coding data, NCDs or anything E-Sys sends to the
  car. The only files it writes in E-Sys's data folder are the [FA / SVT backups](@/tools/fa-svt-backup.md). If it
  fails to load, E-Sys starts normally without names.
- When you open a CAFD that has no definition file yet, the agent saves that CAFD as E-Sys loaded it to
  `workspace\runtime_cafd\` and builds its definition with the same code as **Build definitions**. Everything stays
  on your machine. **Apply names** refreshes these definitions too.
- The agent also adds an **OpenLauncher** section to E-Sys's navigation bar with the
  [tools inside E-Sys](@/tools/_index.md).

If you use a commercial launcher, keep using it as before. It runs its own E-Sys without Open CAFD Map; use
OpenLauncher when you want the names.
