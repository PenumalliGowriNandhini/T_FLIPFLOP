# T_FLIPFLOP
# AIM
To simulate and synthesis T flipflop using vivado.
# Components Required
Vivado 2023.2 software.
# Procedure
STEP:1 Start the vivado software, Select and Name the New project.

STEP:2 Select the device family, device, package and speed.

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and module name and Click Next and then finish button. Type the code and save it.

STEP:5 Select the run simulation and then run Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.

STEP:7 compare the output with truth table.
![image](https://github.com/RESMIRNAIR/T_FLIPFLOP/assets/154305926/74140ea2-0b93-4ffc-b38b-527fb2ece133)
# Truth Table
![image](https://github.com/RESMIRNAIR/T_FLIPFLOP/assets/154305926/1d4afa40-166a-4690-ab1a-179948b9b550)
# Program
```
module tff(clk,reset,t,q);
input clk,reset,t;
output reg q;
always @(posedge clk
begin
if(reset==1)
q=0;
else
begin
if(t==0)
q=q;
else
q=~q;
end
end
endmodule
```
# Output
![image](https://github.com/PenumalliGowriNandhini/T_FLIPFLOP/assets/163722612/c16a7671-fb67-48e4-9454-9b1c106ff0b5)
# Result
Thus the verilog program for T flipflop has been simulated and verified successfully.

