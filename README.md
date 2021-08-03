# Fedar E1

Fedar E1 is a 5-Stage Pipelined (Fetch|Decode|Execute|Memory|Writeback) RV32I RISC-V Core written fully in Verilog.

It has 32 GPIO pins.

![Simulated GTKWave output of the CPU](https://raw.githubusercontent.com/eminfedar/fedar-f1-rv64im/main/gtkwave-image.png)

## How to compile?

1. Open a terminal in `testbench` folder.
2. Run: `run_tests.sh`.
  - The script automatically compile and create files under the `testbench/output/` folder. 
  - And will create `.vcd` files under the `testbench/vcd` folder.
3. Done!

Compilation requires `iverilog` verilog compiler.

You can install iverilog on Debian based distros (like Pardus GNU/Linux or Ubuntu) with this command:
```
sudo apt install iverilog
```

> If you don't want to compile it again, precompiled `.vcd` files are available under the `testbench/vcd`.

## How to open .vcd files?
- Use [GTKWave](https://github.com/gtkwave/gtkwave).

You can install GTKWave on Debian based distros (like Pardus GNU/Linux or Ubuntu) with this command:
```
sudo apt install gtkwave
```
Then double click the files or open with terminal command: `gtkwave file.vcd`.
