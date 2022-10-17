# Transport layer protocols

<details>
  <summary>What is the transmission control protocol or TCP?</summary>

The Transmission Control Protocol (TCP) is a transport protocol that is used on top of IP to ensure reliable transmission of packets.

TCP includes mechanisms to solve many of the problems that arise from packet-based messaging, such as lost packets, out of order packets, duplicate packets, and corrupted packets.

Since TCP is the protocol used most commonly on top of IP, the Internet protocol stack is sometimes referred to as TCP/IP.

Steps:

1. Establish connection - When two computers want to send data to each other over TCP, they first need to establish a connection using a three-way handshake.
2. Send packets of data - When a packet of data is sent over TCP, the recipient must always acknowledge what they received.
3. Close the connection - Either computer can close the connection when they no longer want to send or receive data.

[More >>](https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:the-internet/xcae6f4a7ff015e7d:transporting-packets/a/transmission-control-protocol--tcp)

</details>

<details>
  <summary>What is the user datagram protocol?</summary>

The User Datagram Protocol (UDP) is a lightweight data transport protocol that works on top of IP.

UDP provides a mechanism to detect corrupt data in packets, but it does not attempt to solve other problems that arise with packets, such as lost or out of order packets. That's why UDP is sometimes known as the Unreliable Data Protocol.

UDP is simple but fast, at least in comparison to other protocols that work over IP. It's often used for time-sensitive applications (such as real-time video streaming) where speed is more important than accuracy.

[More >>](https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:the-internet/xcae6f4a7ff015e7d:transporting-packets/a/user-datagram-protocol-udp)

</details>
