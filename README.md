# RV32I Single-Cycle CPU in Verilog

A 32-bit RISC-V processor that implements the RV32I base integer instruction set.
It's a single-cycle design, so every instruction fetches, decodes, executes and
writes back in one clock cycle. It's built from scratch in Verilog and simulated
with Icarus Verilog and GTKWave.

I'm building it one instruction class at a time (R-type, loads, ALU-immediate,
stores, branches, JAL/JALR, LUI/AUIPC), and each class has its own testbench.

**Status:** ALU done and verified. Register file in progress.

**Tools:** Verilog-2005, Icarus Verilog, GTKWave