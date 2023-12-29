# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
# AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

# Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

# Half Adder:
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB  

![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)  

#  Figure -01 HALF ADDER 
# Procedure:

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glowss


Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: AKSHAYA N
RegisterNumber:212223050003 
# program:
 ```
module project_3(sum,carry,a,b); 
input a,b; 
output sum,carry; 
xor sum1(sum,a,b); 
and carry1(carry,a,b); 
endmodule
 ```
# output :
# RTL realization:
![image](https://github.com/Akshaya3563/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155092474/5bf461de-9833-46db-bc5f-63329091a29f)

# TIMING DIAGRAM:
![image](https://github.com/Akshaya3563/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155092474/d94b4d3b-dd48-417d-ba6e-87ee5e8acbae)



#  TRUTH TABLE:
 ![image](https://github.com/Akshaya3563/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155092474/2155a9aa-d152-49a5-bdb1-70012407d0c4)



#  Full Adder:
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BC

![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#  Figure -02 FULL ADDER 

#  Procedure:

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by:AKSHAYA N 
RegisterNumber:212223050003  
# program:
```
module project_3_2(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c;
endmodule
 ```
# OUTPUT:
# RTL realization: 
![image](https://github.com/Akshaya3563/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155092474/4cc194b0-b88b-41ec-b0f0-9a940d4f8c7d)


# TIMING DIAGRAM:
![image](https://github.com/Akshaya3563/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155092474/bc4b1663-6f97-43c2-83a8-d086842e1b7a)
 



#  TRUTH TABLE :
![image](https://github.com/Akshaya3563/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155092474/1a07194a-22f1-41d5-ad9a-13f786a45f18)

 



#  Result:
Thus the given logic functions are implemented and their operations are verified using verilog programming
