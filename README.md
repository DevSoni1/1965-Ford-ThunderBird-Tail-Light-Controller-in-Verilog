# 1965-Ford-ThunderBird-Tail-Light-Controller-in-Verilog
In thunderbird car, the user can give three inputs to indicate signal as LEFT, RIGHT and HAZARD
indication. When LEFT input is given, the first left light (LA) turns ON, then first and second (LA + LB) then all the three (LA+LB+LC), and finally all lights are turn OFF((LA+LB+LC)’). The same case is for RIGHT input signal. For the HAZARD input signal, all the lights will turn ON and OFF continuously, until it becomes 0 again. The HAZARD signal is given highest priority over LEFT and RIGHT to avoid any delays in the emergency situation. If user gives HAZARD at any instant, it should leave the current state and jump quickly to HAZARD state.
The states can be defined in 3-bit wide format ranging from S0(000) to S7(111) defining the status of each lights (LA, LB, LC, RA, RB, RC).
For this, state diagram is designed based on the given parameters and conditions and then Verilog code is written for the same along with TESTBENCH.
The code is written in the Verilog HDL by using MODELSIM (MENTOR GRAPHICS).
This problem is taken from Digital Design by John F. Wakerly but the Verilog program is written by myself own.
