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
### 
Program:

/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
HALF ADDER:
module adder1(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule
FULL ADDER
module expone (a,b,y1,y2,y3,y4,y5,y6,y7);
input a,b;
output y1,y2,y3,y4,y5,y6,y7;
and(y1,a,b);
or(y2,a,b);
not(y3,a);
xor(y4,a,b);
nand(y5,a,b);
nor(y6,a,b);
xnor(y7,a,b);
endmodule

Developed by:RAGUNATH R 
RegisterNumber:22008922
*/
Logic symbol & Truthtable
RTL realization

### Output:

### RTL
HALF ADDER
![image](https://user-images.githubusercontent.com/113915622/211132364-6b0f5ecf-5fc7-40c3-be0b-01415bb64e8f.png)
FULL ADDER:
![image](https://user-images.githubusercontent.com/113915622/211132393-567a48ec-6d8f-4512-a071-9bcd66e47d5b.png)

### TIMING DIAGRAM
HALF ADDER
![image](https://user-images.githubusercontent.com/113915622/211132471-63472769-b41d-48f3-b5a1-042572f6999f.png)
FULL ADDER
![image](https://user-images.githubusercontent.com/113915622/211132509-94f2eb14-fcd7-4610-afd1-eab20e4ccb6d.png)


### TRUTH TABLE
HALF ADDER
![image](https://user-images.githubusercontent.com/113915622/211132546-184fb8d9-8ba2-4178-85b1-405e7cc9b3ad.png)
FULL ADDER
![image](https://user-images.githubusercontent.com/113915622/211132578-6e0754eb-c291-48ca-9c5a-1f424f3ba5ed.png)


### Result:
