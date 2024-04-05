# Multiplexer4to1
# aim
To simulate and synthesis multiplexer using vivado 2023.2

# apparatus
vivado 2023

# procedure
STEP:1 Start the vivado software, Select and Name the New project.

STEP:2 Select the device family, device, package and speed.

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and module name and Click Next and then finish button. Type the code and save it.

STEP:5 Select the run simulation and then run Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.

STEP:7 compare the output with truth table.

# Truth Table
![image](https://github.com/RESMIRNAIR/Multiplexer4to1/assets/154305926/f1dac9e1-e938-4072-bfa9-c17a0a54b7c7)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/Multiplexer4to1/assets/154305926/f8ea8610-f6fc-4de3-a68a-5a9a4cfcd673)

# verilog code
module mux (in0, in1, in2, in3,sel, out);
input in0,in1,in2,in3;
input [1:0] sel;
output reg out;
always@(*)
begin
case (sel)
2'b00: out = in0;
2'b01: out = in1;
2'b10: out = in2;
default: out = in3;
endcase
end
endmodule

# output
![WhatsApp Image 2024-04-05 at 13 27 33_db45180f](https://github.com/lathika024/Multiplexer4to1/assets/165888553/46cf63be-56a2-417a-b32f-a93dba371bd3)



# result
thus the multiplexer4to1 is verified successfully using vivado 2023.2
