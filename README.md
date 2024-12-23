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

![d5557a1c-a713-4ebb-b2f6-74e02b529725](https://github.com/user-attachments/assets/ceaff7c4-6c36-43c8-b2ab-bfe4e96a1a55)


**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

![63840bf0-2060-4de8-b4c5-9e5696331df0](https://github.com/user-attachments/assets/4b69b3d9-d50a-4e1b-a7e9-410e59be111c)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to design a half adder and half subtractor circuit and verify its truth table in quartus using Verilog programming.

Developed by:S.Dharini

RegisterNumber:24002206

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



**RTL:**

Half adder

![exp3 ha logic gate](https://github.com/user-attachments/assets/bfc64623-94ce-4b5f-82aa-a87a0af5ce7d)

Half subtractor

![exp3 hs logic gate](https://github.com/user-attachments/assets/a1ff6e18-be39-47b7-9b89-3b76c593af6c)



**Output:**

Half adder

![exp3 ha op](https://github.com/user-attachments/assets/f177e06a-86f6-4d8c-9779-d272ced8c5db)

Half subtractor

![exp3 hs op](https://github.com/user-attachments/assets/9f1eddb7-67b2-47fc-92e1-dac175c8529b)



**Result:**

Thus the program to design a half adder and half subtractor circuit and verify its truth table in quartus using Verilog programming.

