Chapter 7: Talking to the Outside World — Input, Output, and Serial Communication
Your cpu-brain can crunch numbers and make decisions, but to survive and thrive, it has to interact with the apocalypse world: you need to plug in buttons, displays, keyboards, and mice. This chapter dives deep into how input and output devices work, how they communicate with your machine, and how to build and use them, including a practical mouse project based on your provided materials.

Input and Output Basics
Input devices: Devices that send signals into your computer. Examples: keyboards, mice, switches, sensors.

Output devices: Devices that receive signals. Examples: LEDs, monitors, speakers.

Your CPU doesn't directly “see” these devices. Instead, they connect through interfaces—hardware and protocols that transform signals your machine can understand.

Memory-Mapped I/O and Serial Ports
Input and output devices often appear in the CPU’s memory address space—read and write operations to specific addresses communicate with peripherals (memory-mapped I/O).

Alternatively, special ports (serial or parallel) handle communication.

Serial Communication: The Lifeblood of Peripherals
Serial communication sends data bit by bit over a single wire or pair of wires—like passing notes in a dark alley, one letter at a time.

Protocols like UART, SPI, and I2C define how devices talk, synchronize, and confirm data was received.

Serial saves wiring complexity and is robust enough for mice, keyboards, and networked modules.

How a Mouse Works — Mechanics to Data
Referring to the “build-mouse.pdf” you gave:

Modern mice use sensors (optical or mechanical rollers) to measure motion across two axes.

Each movement translates into digital pulses streamed serially to the CPU.

Buttons are inputs that send discrete signals when pressed or released.

Building Your Own Mouse: Key Concepts
Motion detection via encoders or optical sensors.

A microcontroller or dedicated logic circuits to process sensor signals into meaningful data packets.

Serial transmission of motion and button states via UART or PS/2 protocols.

Practical Project: Build a Basic Serial Mouse Interface
Materials:

Optical sensor or rotary encoder for X and Y movement.

Push-button switches for mouse clicks.

Simple microcontroller or programmable logic device (or discrete logic circuits).

Serial communication interface circuitry.

Instructions:

Connect sensors to measure movement increments.

Encode pulses into serial data streams with direction and magnitude bits.

Add button press signals multiplexed into the data stream.

Implement UART or equivalent serial protocol to send data to your CPU.

Develop CPU-side code or hardware to interpret serial mouse signals into movement actions.

Keyboards and Monitors — More Complex Peripherals
Keyboards send scanned key presses to the CPU, often via serial or parallel protocols. Displays require graphic buffers and data streaming, often via dedicated video cards or simpler LED matrices.