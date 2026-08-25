Chapter 4: Memory and Storage Essentials
Every digital mind, no matter how simple, needs memory—a place to stow bits in-between moments of action. Without memory, a computer is a goldfish: smart, but forgets everything as soon as it happens. Let’s make sure yours can remember.

What Is Memory? Why Does It Matter?
Memory lets your computer store results, instructions, and data—temporarily (RAM) or permanently (ROM, storage).

It makes everything possible: tracking game scores, remembering notes, running programs, and loading the operating system.

The Memory Hierarchy — Fast, Faster, Fastest
Registers: Fastest, tiniest—inside the CPU, used for split-second calculations.

Cache: Holds data the CPU needs soon; speeds things up by reducing RAM fetches.

RAM (Random Access Memory): Your machine’s workspace—stores what’s currently in use.

ROM (Read Only Memory): Stores data or programs that never change—like a circuit’s basic startup directions.

Secondary Storage (Disk, Flash, Tape): Huge, slow, stores everything you’re not using right now but can’t lose.

Analogy: Fast memory is your working hand; RAM is your desk; disk is the file cabinet far from your seat.

RAM vs ROM — Know Your Tools
Feature	RAM	ROM
Volatility	Loses data when off	Keeps data when off
Speed	Fast, for rapid changes	Slower, mostly static
Use	Current, changeable info	Boot code, permanent info
Types of RAM:

SRAM (static, fast, used for cache, keeps data while powered)

DRAM (dynamic, cheap, needs refreshing, used for main system memory)

Types of ROM:

PROM (write once by user)

EPROM/EEPROM (can be erased and reprogrammed with UV light/electricity)

Mask ROM (set at factory)

Building Simple Memory Circuits
Making a Bit: The SR Latch (Bistable Multivibrator)
The most basic memory: two cross-coupled NAND or NOR gates store a single bit (“0” or “1”) as long as power lasts.

Use relays, transistors, or even mechanical switches if electronic parts are scarce.

Making a Byte: Assembling Bits
Link 8 latches to store a byte.

For “random access,” use address lines and logic to read/write each bit separately.

DIY ROM
Use a fixed combination of switches or laser-cut traces—hardwired for unchanging “boot code.”

Early computers used wired “diode matrix” ROMs you could build from salvaged diodes and wire.

DIY RAM (with Caution)
Assemble a small SRAM from relays or transistors—make sure you refresh the bits if using DRAM principles.

Use flip-flops or bistables for ultra-basic digital RAM.

Practical Project: Make a 4-bit Memory Bank
Build four SR latches (using transistors or relays).

Add toggle switches to write values and LEDs to display what’s stored.

Practice: write a pattern, power off, power on, see what’s retained (RAM will forget, ROM won’t).

Survival Tips and Scavenging
Old calculators, toys, and motherboards are goldmines for salvageable RAM/ROM chips.

Practice reading chip part numbers and looking up their functions before trying to use them.

Understanding memory—how to build it, scale it, and use it—means you’re ready to grow your survival computer from a blinking curiosity into a system that actually tracks, stores, and process real “thoughts.” Next: designing the all-important CPU!