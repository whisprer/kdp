Chapter 7: Peripherals and Serial Communication — Connecting Your Zombieproof Computer to the Outside World
You’ve built the brain, the memory, and the basic communication highways inside your zombieproof machine — but what good is a computer that can’t see, hear, or respond? Peripheral devices are your computer’s senses and muscles, allowing it to interact with you and the world.

This chapter demystifies how keyboards, mice, monitors, and other peripherals work, how they communicate using serial and parallel protocols, and guides you through a practical approach to building and interfacing your own mouse, drawing heavily on your provided mouse-building project document.

Input and Output Devices: The CPU’s Interface to Reality
Input Devices: From Physical Action to Digital Signal
Keyboards: Scan matrices to generate unique codes per keypress, sent to the CPU as data packets.

Mice: Detect motion via optical sensors or rollers; buttons register clicks. Movement data encoded and sent to the CPU.

Buttons, switches, sensors: Convert simple physical states into digital signals.

Output Devices: Communicating Back — Displays, LEDs, Speakers
LEDs: Binary on/off lights controlled directly by bits.

Monitors: Use frame buffers and video output protocols to render graphics or text.

Speakers: Convert digital audio streams to sound waves.

Serial Communication: The Language of Peripherals
Most peripherals communicate with the CPU over serial links — sending data one bit at a time on a data line, synchronized by clock signals.

Why Serial?
Minimizes wiring complexity — fewer lines.

Allows multiple devices sharing communication lines (I2C, SPI).

Easier to implement with discrete components in homemade systems.

Key Serial Protocols
UART (Universal Asynchronous Receiver/Transmitter): Common for keyboards and mice; data framed with start, stop, and parity bits.

SPI (Serial Peripheral Interface): Synchronous, faster, with separate clock and data lines; suited for sensors and displays.

I2C (Inter-Integrated Circuit): Multi-device bus using two lines (clock and data) with addressable devices.

The Magic of the Mouse — A Step-by-Step Breakdown
Your mouse is a survival essential for efficient control. Here’s how it works and how to build one:

Mechanics to Data
Optical Sensor or Roller: Detects movement on two axes (X and Y).

Encoders: Convert physical movement into electrical pulses or digital signals.

Buttons: Simple switches that register clicks.

Encoding and Sending Data
Movement and button states are encoded into standardized data packets.

The mouse microcontroller or logic circuit sends this data serially over a communication line (e.g., UART or PS/2 protocol) to the computer.

Building a Zombieproof Mouse
Scavenge optical sensors or rotary encoders from old mice or electronics.

Build simple logic circuits or use a microcontroller to encode motion and clicks.

Implement serial data transmission to link with your CPU.

Practical Project: Constructing Your Own Serial Mouse Interface
Materials Needed:

Optical or rotary sensors for motion detection

Push-button switches

Logic gate ICs or a microcontroller for encoding and communication

Wiring and power supply

Breadboard or perfboard for assembly

Step-by-Step:

Connect sensors to detect X and Y movement; convert to digital pulses.

Connect buttons with debouncing circuits to avoid false signals.

Design or program a data encoder that formats motion and clicks into serial packets.

Transmit packets over a communication line to your CPU, using a protocollike UART.

Develop CPU-side interpreters or hardware to decode mouse data into cursor movement.

Keyboards and Displays — More Complex Yet Vital
Keyboards scan a matrix of switch contacts, generating keycodes conveyed over serial lines.

Displays require memory buffers and dedicated drivers; simpler LED arrays can be directly toggled by the CPU.

Mastering peripherals and serial communication threads the needle from raw binary logic to practical input/output, making your zombieproof computer truly interactive.

Next up: diving into simple operating systems and software layers that bring usability and control.

