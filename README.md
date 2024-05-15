### study-of-basic-gates

**AIM:** 

To study and verify the truth table of logic gates in Quartus II using Verilog programming.

**Equipments Required:**

Software – Quartus prime 

**Theory**

Introduction Logic gates are the basic building blocks of any digital system. Logic gates are electronic circuits having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic. Based on this, logic gates are named as

AND gate OR gate NOT gate NAND gate NOR gate Ex-OR gate Ex-NOR gate

**AND gate**

The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB
Y= A.B

**OR gate** 

The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation.
Y= A+B

**NOT gate**

The NOT gate is an electronic circuit that produces an inverted version of the input at its output. It is also known as an inverter. If the input variable is A, the inverted output is known as NOT A. This is also shown as A' or A with a bar over the top, as shown at the outputs.
Y= A'

**NAND gate**

This is a NOT-AND gate which is equal to an AND gate followed by a NOT gate. The outputs of all NAND gates are high if any of the inputs are low. The symbol is an AND gate with a small circle on the output. The small circle represents inversion.
Y= (AB)’

**NOR gate**

This is a NOT-OR gate which is equal to an OR gate followed by a NOT gate. The outputs of all NOR gates are low if any of the inputs are high. The symbol is an OR gate with a small circle on the output. The small circle represents inversion.
Y= (A+B)’

**Ex-OR gate**

The 'Exclusive-OR' gate is a circuit which will give a high output if either, but not both of its two inputs are high. An encircled plus sign (⊕) is used to show the Ex-OR operation.
Y= A⊕B

**Ex-NOR gate**

The 'Exclusive-NOR' gate circuit does the opposite to the EX-OR gate. It will give a low output if either, but not both of its two inputs are high. The symbol is an EX-OR gate with a small circle on the output. The small circle represents inversion.
Y= A⊕B

**Procedure** 

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**PROGRAM**
```
Program for logic gates and verify its truth table in quartus using Verilog programming

Developed by: Adhl Hameed
Register Number: 212223050002
#AND-GATE
module andgate(a,b,e);
input a,b;
output e;
assign e = (a & b);
endmodule

#NOT-GATE
module notgate(a,e);
input a;
output e;
assign e = ~(a);
endmodule

#OR-GATE
module orgate(a,b,e);
input a,b;
output e;
assign e = (a | b);
endmodule

#NAND-GATE
module nandgate(a,b,e);
input a,b;
output e;
assign e = ~(a & b);
endmodule

#NOR-GATE
module norgate(a,b,e);
input a,b;
output e;
assign e = ~(a | b);
endmodule

#XNOR-GATE
module xnorgate(a,b,e);
input a,b;
output e;
assign e = ~(a ^ b);
endmodule

#XOR-GATE
module xorgate(a,b,e);
input a,b;
output e;
assign e = (a ^ b);
endmodule
```

**Logic symbol & Truthtable**

#AND-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/fe4a64b3-604a-44b7-91ef-f6e9b2a9ff9a)

#NOT-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/a2cb7ef0-8e49-4086-b698-b5572783616d)

#OR-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/1b908795-8695-40ee-8866-393463fce0c1)

#NAND-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/ca180f4a-2b06-41f4-8a24-ba35340cb476)

#NOR-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/766db8fa-4a33-4ef4-93d2-0029397b0c5a)

#XNOR-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/b008e8b1-878e-412f-8f43-80328621bd00)

#XOR-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/39099967-a65b-42b3-90f9-439ffb3049cb)

**RTL realization Output:** 

#AND-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/0ca3a9a3-0b07-48c7-ba9e-5ad1d2b41bf1)


#NOT-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/51e320e6-4596-43cc-8d2d-0416070edd3e)


#OR-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/2c66aafe-3f96-4723-8818-bbfd17bbe4da)


#NAND-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/8d1eac00-5176-4785-b3a1-b1fae9d8546e)


#NOR-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/0a802d51-650b-4f97-adc6-f51dcb55c21b)


#XNOR-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/7b5a72c0-47d8-424b-8972-0eb6a618329b)


#XOR-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/8f07050c-21f3-4156-9cff-ddf9d1b5a0d0)


**RTL**

#AND-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/4dadf25f-6dc8-400c-b8d6-a00db846b163)


#NOT-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/b0af1e0a-6c0e-4976-ad14-f1497f4c0137)


#OR-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/f22dec0d-f119-411d-a263-570757a26f1f)


#NAND-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/a401cc5c-4a25-456e-b9de-a3a6ce4722d0)


#NOR-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/fd386d7b-7030-4c16-92f5-c6429cc8ac40)


#XNOR-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/bcba77b6-8689-4c42-b528-f577c9d0ee0e)


#XOR-GATE

![image](https://github.com/adhlhameed/study-of-basic-gates/assets/168260238/c024e32d-4127-4a3a-9132-9d29642e3965)

**Result:**
Thus, the programs have been executed.

