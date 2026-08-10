Chapter 6: Memory Integration — Bringing Storage to Your CPU
Welcome, woflfren, to the next huge milestone. Your CPU, as brilliant as it is, is just a brain with no memory. Without a way to store programs and data beyond a fleeting moment, your zombieproof computer is a roaring beast with no shelter to keep its secrets safe.

This chapter untangles memory’s mysteries — from basic RAM concepts to address decoding and connecting your CPU to live memory chips. We’ll cover why different memory types exist and how to build the bus and control systems that let the CPU talk clearly to the memory jungle.

Why Memory Matters
Memory is your computer’s archive and blank slate. It holds:

The instructions (programs) your CPU must execute

The data the CPU manipulates

Temporary workspace for intermediate calculations

Without memory, the processor is adrift, with no instructions to fetch, no data to operate on, no way to save results.

Types of Memory at a Glance
RAM — Random Access Memory
This is the key workbench—fast, volatile, and changeable. RAM lets the CPU read or write any byte nearly instantly.

Volatile: Data disappears if power cuts (bring backup!).

Built as arrays of bits stored in flip-flops or capacitors.

ROM — Read-Only Memory
Permanent instruction storage, critical for bootstrapping your system.

Non-volatile, retains data without power.

Useful for firmware, startup code, or fixed lookup tables.

Memory-Mapped I/O
In zombieproof computers, peripherals like LEDs or switches are accessed as if they were memory addresses — simplifying wiring and programming.

Address Space and Address Lines
Memory chips are organized by addresses — unique numbers representing each byte or word.

The width of your address bus determines maximum memory: 
2
N
2 
N
  addresses for an 
N
N-bit bus.

Example: A 4-bit address line addresses 
2
4
=
16
2 
4
 =16 memory locations.

More address lines, more memory, but also more wiring.

Decoding Addresses — Choosing Who Listens
Your CPU uses address lines to talk to many memory modules or devices. How does it ensure only the right chip listens?

The answer: Address decoding circuits — built from logic gates.

These decode a subset of address bits to enable a single memory chip at a time.

Use NAND gates or decoders to generate chip select signals.

Simple Decoder Example
If bits 
A
3
−
A
0
A3−A0 select memory location, a decoder that recognizes bits 
A
7
−
A
4
A7−A4 determines which module to enable.

Only when a module's address bits match does it activate its chip select line.

This avoids bus conflicts, where multiple chips drive data lines simultaneously.

The Bus — The Data Highway
Your CPU and memory share physical wires forming a bus:

Data bus: Transfers data both ways.

Address bus: Carries the address of memory operations.

Control bus: Contains read/write signals and chip enables.

Avoiding Collisions with Tri-State Logic
Bus lines must be driven by only one device at once.

Memory chips use tri-state buffers to release data lines (high impedance state) when not selected.

Enables multiple devices to share the bus cleanly.

Interfacing CPU and Memory — The Workflow
CPU places address on address bus.

Address decoder activates matching module.

CPU asserts read or write control signals.

For read, memory outputs data on data bus; for write, CPU sends data on bus into memory.

Done — the CPU stores or retrieves information.

Building Your First Memory Interface — Survival Project
Components
A simple RAM chip or register arrays

NAND gates for address decoding

Tri-state buffers or equivalent for bus control

Wiring, breadboard, power source

Procedure
Wire CPU address lines into decoder gates for memory select.

Connect data lines with tri-state buffers ensuring only one driver at a time.

Build and test read/write cycles with simple CPU instructions.

Use LEDs or logic analyzers to monitor bus data and control signals.

Timing — Synchronizing Memory Access
Memory read/write must align with CPU clock.

Add delay cycles if memory is slow.

Ensure control signals activate at precise clock phases to avoid data corruption.