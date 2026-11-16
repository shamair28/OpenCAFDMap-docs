+++
title = "First start"
weight = 3
+++

1. Open **OpenLauncher** (the shortcut, or `OpenLauncher.bat`).
2. Check the **E-Sys folder** (found automatically if it's in the usual place) and the **main series**
   (`G020` covers G20/G21/G22/G23/G26/G28/G8x). Leave **psdzdata** empty to use the one E-Sys is set up with.
   Press **Save settings**.
3. Press **Start E-Sys with Open CAFD Map**, connect or open your coding data as usual, and open a CAFD: the tree
   shows names and labels.
   - The first start reads your psdzdata's FA→FP mapping once (about 20 seconds), so option codes like `SA5AC`
     show up.
   - A CAFD opened for the first time shows BMW's untrimmed names straight away. Within a few seconds its full
     definition is built in the background and the tree updates by itself. Later opens are instant.
4. Optional: press **Build definitions** to decrypt and index all of your psdzdata's CAFDs for that series. It can
   take a while. The [BimmerCode Backup Editor](@/backup-editor/_index.md) and the command-line tools need it;
   E-Sys doesn't.

After editing names, press **Apply names** (a few seconds), then reopen the CAFD in E-Sys.
