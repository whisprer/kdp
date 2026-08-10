Chapter 4a: Foundations of Memory and Data Routing — Flip-Flops, Registers, and Multiplexers
Your journey into building a zombieproof CPU demands more than knowing what a flip-flop or multiplexer is—it requires understanding exactly how these are made with simple gates, how they store and pass data reliably, and how timing controls the flow. This chapter is your guide to these vital building blocks.

Flip-Flops: The Tiny Memory Cells
Flip-flops are circuits that remember a single bit by feeding outputs back into inputs, creating stable states.

Constructing an SR Flip-Flop
Use two cross-coupled NOR gates to build a basic SR (Set-Reset) flip-flop.

Show truth table, circuit diagram, and explain stable and forbidden states.

D Flip-Flop: Capturing Data on the Clock Edge
Add gating logic for synchronized data capture; avoid unstable conditions.

Use NAND gates and latches to form a D flip-flop.

Practical circuit: Wiring a D flip-flop on a breadboard using NAND gates and timing it with your clock.
Registers: Collections of Flip-Flops
Explain how to combine multiple flip-flops for multi-bit registers with load enable signals:

Design 4, 8 bit registers from D flip-flops.

Implement load control so data is stored only at certain clock pulses.

Shift Registers: Moving Bits Along a Chain
Show classic serial-in, serial-out design from flip-flops.

Explain shifting data bit by bit on clock edges with practical timing diagrams.

Discuss parallel-in/out variations.

Multiplexers: Circuit Switchboards
Define selector inputs and how AND/OR gate combinations multiplex signals.

Build 2-to-1 and 4-to-1 muxes from basic gates.

Explain how link multiplexers to registers and ALU datapaths.

Practical Survival Project
Build and test a 4-bit register with load control using your flip-flop circuits.

Construct a 2-to-1 multiplexer and test data selection between two registers.