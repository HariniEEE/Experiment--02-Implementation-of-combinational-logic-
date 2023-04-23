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
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

PROGRAM 1:

module exp;

input a,b,c,d;

output f1,f2,f3;

assign f1=(~c&~b&~a);

assign f2=(~d&~c&~a);

assign f3=(c&~(~b)&~a);

assign f=f1&~f2&~f3;

endmodule

PROGRAM 2:

module expfourtwo(a,b,c,d,f);

input a,b,c,d;

output f;

wire f1,f2,f3,f4;

assign f1=c&(~b)&a;

assign f2=d&(~c)&a;

assign f3=c&(~b)&a;

assign f4=~(f1|f2|f3);

not(f,f4);

endmodule


Developed by: Harini E
RegisterNumber:  212222050017
*/

## Output:

##Logic Diagram:

PROGRAM 1
![logic 1](https://user-images.githubusercontent.com/128949246/233824832-83385e4a-d43a-4d66-a4a4-6041f29b3586.jpeg)

PROGRAM 2
![logic 2](https://user-images.githubusercontent.com/128949246/233824847-045d50b3-4346-4c97-845d-878769f380d5.jpeg)

##Truth table:

PROGRAM 1
![truth 1](https://user-images.githubusercontent.com/128949246/233824921-2596eaac-15d8-44b6-9adb-08f14b26fb86.jpeg)

PROGRAM 2
![truth 2](https://user-images.githubusercontent.com/128949246/233824949-2671c989-dba5-485f-bf6b-73828b9b7d58.jpeg)


## Timing Diagram

PROGRAM 1
![timing 1](https://user-images.githubusercontent.com/128949246/233824770-023e8361-86e7-4ae3-a830-f6f897db2e99.jpeg)

PROGRAM 2
![timing 2](https://user-images.githubusercontent.com/128949246/233824787-b037286e-9778-480c-9d82-2f2f252c6966.jpeg)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
