Part 1: Half and Full Adders — The Building Blocks of Binary Math
Introduction: Why Adders Matter
Addition is fundamental for all computing tasks, from math to decision-making. Adders let computers sum numbers bit by bit.

Half Adder: Adding One-Bit Numbers
Inputs: Two bits (
A
A and 
B
B).

Outputs:

Sum (S): The bit-wise sum without carry.

Carry (C): The bit to carry over to the next digit.

Boolean expressions:

S
=
A
⊕
B
S=A⊕B (XOR)

C
=
A
⋅
B
C=A⋅B (AND)

Circuit:

Use an XOR gate for Sum, AND gate for Carry.

Full Adder: Adding with Carry
Inputs: Two bits plus a carry-in bit 
C
i
n
C 
in
 .

Outputs:

Sum (S):

Carry-out 
C
o
u
t
C 
out
 :

Boolean expressions:

S
=
A
⊕
B
⊕
C
i
n
S=A⊕B⊕C 
in
 

C
o
u
t
=
(
A
⋅
B
)
+
(
C
i
n
⋅
(
A
⊕
B
)
)
C 
out
 =(A⋅B)+(C 
in
 ⋅(A⊕B))

Circuit: Combine two half adders and an OR gate.

Cascading Adders for Multi-bit Operations
Combine 
n
n full adders for 
n
n-bit addition, carrying 
C
o
u
t
C 
out
  to next 
C
i
n
C 
in
 .

Example: 4-bit adder from 4 full adders chained.

Hands-on Project: Build Your Own Adders
Using basic gates, build a half adder and a full adder on breadboard or using logic gate simulators.

Test all input combinations to verify outputs.