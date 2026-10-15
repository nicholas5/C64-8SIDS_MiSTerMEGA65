# C64-8SIDS_MiSTerMEGA65

This repository was created to explore the feasibility of synthesizing 8 SID instances in the MiSTerMEGA65 C64 core.

This is intentionally a trial branch and not a finished 8-SID implementation.
The key change is in `rtl/sid/sid_top.sv`, where the SID array count is forced to 8 so the design can be synthesized and resource usage can be checked.

Goals:
- estimate FPGA utilization for 8 SID cores
- validate whether the current core architecture can tolerate the additional SID logic
- identify the next required changes for bus decoding and audio routing

Important:
- This repo is for experimentation only.
- The core still requires follow-up work in address decode, filter configuration, audio mixing, and menu/firmware support before it behaves like a true 8-SID C64 implementation.
