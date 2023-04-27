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
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: jeevitha.E
RegisterNumber:212222230054 

HALF ADDER:
module fulladd (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule

Full adder program:

module fulladd (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
```

Logic symbol & Truthtable
RTL realization

### Output:
### RTL
### HALF ADDER:
![halfadd](https://user-images.githubusercontent.com/118708245/231667707-164af9d3-eeb3-42a8-8958-89bb2aff3c39.png)
### FULL ADDER:
![full add](https://user-images.githubusercontent.com/118708245/231668051-7f1ee89b-03e2-4c1f-8c16-900ed0488836.png)

### TIMING DIAGRAM
### HALF ADDER:

![half add](https://user-images.githubusercontent.com/118708245/231670748-ea858d29-72b4-45f8-bfff-5808e0da2a9c.png)

### FULL ADDER:

![Screenshot 2023-04-16 223113](https://user-images.githubusercontent.com/118708245/232328362-297324fe-4718-4148-bf1b-b4c7f84f328b.png)

### TRUTH TABLE:
# HALFADDER:
![Screenshot 2023-04-16 223219](https://user-images.githubusercontent.com/118708245/232328455-a8309e5e-cd58-4ad3-9b77-ee82bc807471.png)
# FULL ADDER:
![Screenshot 2023-04-16 223321](https://user-images.githubusercontent.com/118708245/232328494-65fb5f74-e38f-4569-b400-8a7da94cbdde.png)
 
### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
