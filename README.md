# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
# AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

# Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

# Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

# Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

# Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
# Program:

### Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: SANDHIYA R

RegisterNumber: 212222230129  

### Half adder program:
 ```
module fulladd (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule
```
### Full adder program:
```
module fulladd (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
 ```

# Output:
### Half Adder
![image](https://user-images.githubusercontent.com/113497571/229456720-2890d884-5a7b-49ad-b938-7285950fcc11.png)
### Full Adder
![image](https://user-images.githubusercontent.com/113497571/229456871-16a6d9d8-b27c-4195-a8a6-aec37c5dd1e4.png)

### RTL
### Half Adder
![image](https://user-images.githubusercontent.com/113497571/229457001-bce93ddb-6296-409d-bf51-831bcaa2a50b.png)
### Full Adder
![image](https://user-images.githubusercontent.com/113497571/229457166-3b7ba198-5093-411c-bda0-2a7b400f5b2f.png)

### TIMING DIAGRAM
### Half Adder
![image](https://user-images.githubusercontent.com/113497571/229457256-de0aa245-7d3d-4f1e-ba19-6b3c0e4cddeb.png)
### Full Adder
![image](https://user-images.githubusercontent.com/113497571/229457336-76f9b77c-ea93-4c34-8c3d-5480e069bab5.png)
### TRUTH TABLE 
### Half Adder
![image](https://user-images.githubusercontent.com/113497571/229457469-b30c0bb7-19b0-498f-b373-c5e4fe7bd4ee.png)
### FULL Adder
![image](https://user-images.githubusercontent.com/113497571/229457555-bf7666bb-37be-4b84-a264-b3f6f0057bcd.png)

# Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
