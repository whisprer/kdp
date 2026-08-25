Chapter 9: Networking Your Zombieproof Computer — From isolated fortress to connected survivor

So your zombieproof computer can think, remember, and interact with you and the peripherals in your bunker. But survival isn’t just about solo strength — it’s about community, information flow, and coordinated defense. Networking brings your machine from a lone warrior to part of a resilient digital tribe.

This chapter explores how to build simple networking capabilities into your zombieproof rig, teaching you about basics of network hardware, protocols, and how to actually wire two or more machines together to share messages or data. We’ll cover foundational concepts like packet communication, serial and parallel links, and practical interfaces.

Why Network at All?
A network lets multiple computers:

Share data and resources

Distribute processing loads

Communicate in real-time or asynchronously

Help rebuild digital civilization post apocalypse

The Basics of Networking Hardware
Physical Mediums
Wired: Ethernet cables, serial links, USB, or simple point-to-point wiring.

Wireless: Radio (Wi-Fi, Bluetooth), though more complex and power-hungry.

Network Interface
An interface chip or module handles physical layer tasks, encoding data onto the medium and collecting signals.

Data Formats and Packets
Network communication sends data in packets—chunks with headers, payloads, and checksums.

Headers include addressing info so the data reaches the right machine.

Payload is actual data content.

Checksums help detect errors.

Communication Protocols
Protocols are agreed “languages” machines use to talk.

TCP/IP: The Internet’s backbone, complex but ubiquitous.

Simple Serial Protocols: Easy to implement for two-machine or small networks.

Example: RS-232 or UART-based communication, with start bits, stop bits, and parity checks.

Wiring Your Network — Point-to-Point Serial Link Example
Connect two zombieproof computers via serial ports.

Use UART modules or logic circuits to send and receive bytes.

Implement basic handshake and flow control to avoid data loss.

Practical Project: Simple Network Link Between Two Machines
Wire RX (receive) of one to TX (transmit) of the other and vice versa.

Ensure matching baud rates and protocol parameters.

Create sending and receiving routines in your OS or firmware.

Test by exchanging simple messages or commands.

Beyond Basics — Multi-node Networks and Switching
Using multiplexers and bus protocols to extend beyond point-to-point.

Packet routing and addressing schemes enable scalable networks.

Consider timing, collision detection, and retransmission strategies.

Networking transforms your zombieproof machine from a solitary sentinel into a connected ally in the fight for survival. Ready to wire the next chapter of your post-apocalyptic revolution?