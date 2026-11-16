+++
title = "Before you restore"
weight = 3
+++

1. **Signature.** Each backup contains the ECU's NCD signature block (for example FLM2 37F1, BDC 3456, MGU 3016).
   BimmerCode computes a new one on every change it makes; this editor doesn't compute or forge signatures. Edited
   backups therefore carry the **source backup's signature**.
   - If BimmerCode re-signs when it restores, restoring works normally.
   - If it writes the stored blocks as they are, the ECU may refuse the coding or report a coding fault. Restoring
     the unedited original backup returns the ECU to its previous state.
   - **Try one low-risk change first** (for example a head-unit display option) before anything safety- or
     drive-related.
2. **Same software only.** A backup applies to the CAFD version it was read from. After an ECU update, take a fresh
   BimmerCode backup and edit that.
3. **Multi-ECU features** often need a change in several ECUs (for example a drive mode in the BDC *and* the head
   unit). Make and restore every backup involved.
4. **Names come from the definition DB:** community names, cheat sheets you imported locally, and labels dynamically
   calculated from BMW's coding rules (`[SA9XA]` = the factory option that normally selects that value).
