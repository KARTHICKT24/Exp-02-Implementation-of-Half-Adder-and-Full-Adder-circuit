# NAME:KARTHICK KISHORE.T
# REF NO:212223220042
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
# Program:

                     Half adder program:
module HalfAdder(A,B,sum,carry);
input A,B;
output sum,carry;
assign sum= A^B;
assign carry = A&B;
endmodule
                        Full adder program:
module FullAdder(A,B,Cin,sum,carry);
input A,B,Cin;
output sum,carry;
assign sum= A^B^Cin;
assign carry = (A&B)|((A^B)&Cin);
endmodule


# RTL:
HALF ADDER:


![267697209-71a3eb96-da66-46de-a2d9-1645d8ee54d1](https://github.com/KARTHICKT24/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149347526/90cf18d5-0c85-494b-88e2-d61133331cb0)


FULL ADDER:


![267697282-9530133a-8b2e-4f16-b0f8-0f7e22ec9e2a](https://github.com/KARTHICKT24/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149347526/554d0be1-b259-4cc4-ab20-ae9b6285b8ce)

# TRUTH TABLE:
HALF ADDER:


![271368907-7c6ac847-6a3f-489d-94ad-2e287ccd0222](https://github.com/KARTHICKT24/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149347526/539f0bec-e9f6-4474-a819-d9a834684720)

FULL ADDER:


![271368953-1e0a0b0c-ae7b-4de3-8519-f007cf7211db](https://github.com/KARTHICKT24/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149347526/0f851323-c51f-402f-bd84-76b0a5f2a9c0)


# WAVEFORM:
HALF ADDER:

![267697561-218a4305-8c84-4935-916f-ec9d19dbde14](https://github.com/KARTHICKT24/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149347526/b3a527b5-5fde-4b1a-9fb4-e612d1384c3d)

FULL ADDER:

![267697631-7b3e726c-da2c-4c14-a095-7c14956bae56](https://github.com/KARTHICKT24/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149347526/b57c2ab0-f24e-4764-ae56-13fc9f1b567c)




### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
