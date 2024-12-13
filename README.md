# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

i)HALF ADDER


![half adder](https://github.com/user-attachments/assets/90c511cb-dbaf-4741-946b-0996b1cd2b3b)


ii)HALF SUBTRACTOR

![half_sub](https://github.com/user-attachments/assets/2a8f70a6-9eb8-4230-90b2-a438f3dbb7a6)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:MUKESH R
RegisterNumber:24000238
*/
```
i)HALF ADDER

module ha(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule

ii)HALF SUBTRACTOR

module hs(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule
```
**RTL**

i)HALF ADDER


![exp03f1](https://github.com/user-attachments/assets/d7d189e9-91a2-4e35-a550-897ab69a4b4f)

ii)HALF SUBTRACTOR


![exp03f2](https://github.com/user-attachments/assets/1e97a70e-625f-4ab7-b1f2-02343c9b4ac8)

**Output/TIMING Waveform**

i)HALF ADDER


![output 03-1](https://github.com/user-attachments/assets/c8c09e33-91e4-4d14-9151-23f2494b1357)


ii)HALF SUBTRACTOR


![output03-2](https://github.com/user-attachments/assets/f5e81420-5013-4f77-b7c6-0c2406188d21)


**RESULT**

A half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.
