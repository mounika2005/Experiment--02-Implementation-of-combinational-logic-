## Developed by: Lakshmi mounika
## RegisterNumber:  23004124
# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy

## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime

## Theory
## Procedure

## Program:
module experiment2(A,B,C,D,F1);
input A,B,C,D;

output F1;

wire x1,x2,x3,x4,x5;


assign x1=(~A)&(~B)&(~C)&(~C);

assign x2=(A)&(~D)&(~D);

assign x3=(~B)&(C)&( ~D);

assign x4=(~A)&(B)&(C)&(D);

assign x5=(B)&(~C)&(~D);

assign F1=x1|x2|x3|x4|x5;
endmodule

## RTL realization
![Screenshot 2023-11-26 173053](https://github.com/mounika2005/Experiment--02-Implementation-of-combinational-logic-/assets/145633112/21e1ae21-bf4e-4cf6-990c-04303e40d522)
# Truth table:
![Screenshot 2023-11-26 173233](https://github.com/mounika2005/Experiment--02-Implementation-of-combinational-logic-/assets/145633112/c6468b54-7ec8-4a38-b959-64b7df34c7e3)
# Timing Diagram:
![Screenshot 2023-11-26 173342](https://github.com/mounika2005/Experiment--02-Implementation-of-combinational-logic-/assets/145633112/4640dcf3-91e4-42c8-bf85-e0d7d05d2b63)
## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
