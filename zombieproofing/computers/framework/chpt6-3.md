Part 3: Registers and Shift Registers — Data Storage and Movement
What Are Registers?
Small, fast memory locations inside the CPU holding data temporarily.

Used for operands, intermediate results, and control data.

Much faster than main memory (RAM).

Building a Basic Register
Use flip-flops (bistable circuits) to store a single bit.

Combine 8 flip-flops for an 8-bit register (1 byte).

Control lines:

Load (write) enable: Decide when to store new data.

Clear/reset: Empty the register.

Output enable: Send stored data to CPU buses.

Flip-Flops: The Building Blocks
SR flip-flop: Simple memory with Set and Reset inputs.

D flip-flop: Captures input at clock edge—key for synchronous registers.

JK and T flip-flops: Variations useful for counters and toggles.

Shift Registers: Moving Data Bit by Bit
Chains of flip-flops that move data one bit at a time on each clock pulse.

Useful for serial communication, multiplication, division, and buffering.

Types:

Serial-in, serial-out (SISO)

Serial-in, parallel-out (SIPO)

Parallel-in, serial-out (PISO)

Parallel-in, parallel-out (PIPO)

Building a Shift Register
Connect several D flip-flops in series.

Use a clock pulse to “shift” bits along the chain.

Control mechanisms for loading and reading data.

Practical Project: Build a 4-bit Register and Shift Register
Use flip-flop ICs or breadboarded transistor flip-flops.

Test loading and retrieving data.

Use clock pulses to shift data through the register.

With registers and shift registers built, storage and data movement inside your CPU become tangible and controllable. Next up: combining all these elements and control signals to form the bits of your CPU — the stepping stones for instruction registers and the program counter. 