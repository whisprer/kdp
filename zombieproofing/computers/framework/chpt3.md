Chapter 3: Digital Logic from the Ground Up
All the world’s computing power comes down to one thing—making simple “yes/no” decisions, millions of times a second. Welcome to the realm of binary, where 1s and 0s rule, and a handful of logic gates unlock everything from calculators to supercomputers.

Understanding Binary: The Language of Electronics
Computers use binary because it’s reliable and easy to implement—electricity is either “flowing” (1) or “not” (0).

Binary numbers build up all information, from text and images to math.

Example: The number 6 in binary is 
110
2
110 
2
 , which means 
1
×
2
2
+
1
×
2
1
+
0
×
2
0
1×2 
2
 +1×2 
1
 +0×2 
0
 .

Boolean Algebra: The Math of Logic
Boolean algebra describes how binary values interact.

Main operators: AND, OR, NOT, NAND, NOR, XOR, XNOR.

Every digital operation, from addition to decision-making, can be broken into these gate operations.

Building Basic Logic Gates
AND Gate
Outputs 1 only if both inputs are 1.

DIY: Two switches in series—a lamp lights only when both are pressed.

OR Gate
Outputs 1 if either input is 1.

DIY: Two switches in parallel—the lamp lights if either (or both) are pressed.

NOT Gate (Inverter)
Reverses input: 0 becomes 1, 1 becomes 0.

DIY: Use a transistor circuit—when input is high, the output is pulled low, and vice versa.

NAND, NOR, XOR, XNOR
NAND: NOT + AND—output is 0 only if both inputs are 1.

NOR: NOT + OR—output is 1 only if both inputs are 0.

XOR: Outputs 1 if only one input is 1.

XNOR: Outputs 1 if both inputs are the same.

Hands-On: Making a NAND Gate from Scratch
Use transistors, or even relays (for large, visible builds).

Test your gate by verifying its truth table: Try out all possible input combinations and see if the output matches expectations.

Building and Testing Circuits
Draw simple diagrams (circuit schematics) to keep organized.

Test each gate with a battery, switches, and LEDs—if it doesn’t work, check connections and test components.

Combine gates—e.g., make an XOR gate by combining AND, OR, and NOT gates.

Why Logic Gates Matter
Every function in a computer—from memory to arithmetic to controlling robots—starts with logic gates.

Mastery of gates lets you design bigger modules: adders, counters, memory, even full CPUs.

Chapter Project: Build a Logic Tester
Make a test board that lets you try out all your homemade gates quickly.

Include labeled switches and LEDs.

Use a multimeter (or DIY tester) to check logic levels at each point.

Digital logic is the essential bridge between raw electronics and the “thinking” part of computers. With these gates solidly in your toolkit, you’re ready to build calculators, timers, or jump into the wild world of adders and arithmetic—coming up next