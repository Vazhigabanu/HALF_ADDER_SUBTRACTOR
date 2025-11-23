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
<img width="424" height="249" alt="half sub truth table" src="https://github.com/user-attachments/assets/13158fee-24e1-4c4b-a5d1-db4beb40c4e1" />
<img width="436" height="248" alt="half sub2 truth table" src="https://github.com/user-attachments/assets/21fc7e08-40e9-4a58-83e5-38d04c5fc1ca" />

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:s.vazhiga banu

RegisterNumber:25014707

```
i) module expt3(a,b,sum,carry); 
input a,b; 
output sum,carry; 
assign sum= (a ^ b); 
assign carry= ( a & b); 
endmodule 

ii) module expt3(a,b,difference,borrow); 
input a,b; 
output difference,borrow; 
assign difference= (a ^ b); 
assign borrow= ( ~a & b); 
endmodule
```
**RTL Schematic**
<img width="1920" height="1200" alt="Screenshot 2025-11-23 220200" src="https://github.com/user-attachments/assets/4a754fd6-222a-473b-9812-074100914297" />
<img width="1920" height="1200" alt="Screenshot 2025-11-23 220354" src="https://github.com/user-attachments/assets/262f181b-bb2b-40ea-8974-e8b24e524c47" />


**Output/TIMING Waveform**
<img width="1845" height="954" alt="Screenshot 2025-11-23 215706" src="https://github.com/user-attachments/assets/88f95a31-27e1-4e8f-897e-ffc2114311b8" />
<img width="1851" height="959" alt="Screenshot 2025-11-23 215733" src="https://github.com/user-attachments/assets/87d82cb2-292b-4278-aa66-f0d0a8aee189" />


**Result:**
Thus a basic neural network regression model for the given dataset is written and executed successfully
