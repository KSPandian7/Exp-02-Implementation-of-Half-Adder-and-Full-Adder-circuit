# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### Program:
```/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: KULASEKARAPANDIAN K
RegisterNumber:  212222240052

HALF ADDER

module Adder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule

FULL ADDER

module FullAdder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule
*/
```

Logic symbol & Truthtable
RTL realization

### Output:

### RTL
![image](https://user-images.githubusercontent.com/113496887/233279258-8ee55284-cf0b-422a-822c-b8c2e1ed1db4.png)
![image](https://user-images.githubusercontent.com/113496887/233279404-607e2407-353f-4b90-9d7c-4862818c36f9.png)



### TIMING DIAGRAM
![image](https://user-images.githubusercontent.com/113496887/233279756-50d5005b-7119-4bfc-b4a9-96900cae97ae.png)
![image](https://user-images.githubusercontent.com/113496887/233279830-658340b7-59f5-42df-850d-ad9a817a1f50.png)



### TRUTH TABLE 
![image](https://user-images.githubusercontent.com/113496887/233280003-a40dcaa7-e300-40de-89dc-17e574a97324.png)


### Result:
Thus, a half adder and full adder circuit is designed to verify its truth table in Quartus using Verilog programming.


