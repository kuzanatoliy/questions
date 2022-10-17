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

<details>
  <summary>What difference between TCP and UDP?</summary>

| Basis                    | Transmission control protocol (TCP)                                                                                                                                                                                    | User datagram protocol (UDP)                                                                                                                                                                                                              |
| ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Type of Service          | TCP is a connection-oriented protocol. Connection-orientation means that the communicating devices should establish a connection before transmitting data and should close the connection after transmitting the data. | UDP is the Datagram-oriented protocol. This is because there is no overhead for opening a connection, maintaining a connection, and terminating a connection. UDP is efficient for broadcast and multicast types of network transmission. |
| Reliability              | TCP is reliable as it guarantees the delivery of data to the destination router.                                                                                                                                       | The delivery of data to the destination cannot be guaranteed in UDP.                                                                                                                                                                      |
| Error checking mechanism | TCP provides extensive error-checking mechanisms. It is because it provides flow control and acknowledgment of data.                                                                                                   | UDP has only the basic error checking mechanism using checksums.                                                                                                                                                                          |
| Acknowledgment           | An acknowledgment segment is present.                                                                                                                                                                                  | No acknowledgment segment.                                                                                                                                                                                                                |
| Sequence                 | Sequencing of data is a feature of Transmission Control Protocol (TCP). This means that packets arrive in order at the receiver.                                                                                       | There is no sequencing of data in UDP. If the order is required, it has to be managed by the application layer.                                                                                                                           |
| Speed                    | TCP is comparatively slower than UDP.                                                                                                                                                                                  | UDP is faster, simpler, and more efficient than TCP.                                                                                                                                                                                      |
| Retransmission           | Retransmission of lost packets is possible in TCP, but not in UDP.                                                                                                                                                     | There is no retransmission of lost packets in the User Datagram Protocol (UDP).                                                                                                                                                           |
| Header Length            | TCP has a (20-60) bytes variable length header.                                                                                                                                                                        | UDP has an 8 bytes fixed-length header.                                                                                                                                                                                                   |
| Weight                   | TCP is heavy-weight.                                                                                                                                                                                                   | UDP is lightweight.                                                                                                                                                                                                                       |
| Handshaking Techniques   | Uses handshakes such as SYN, ACK, SYN-ACK It’s a connectionless protocol i.e.                                                                                                                                          | No handshake                                                                                                                                                                                                                              |
| Broadcasting             | TCP doesn’t support Broadcasting.                                                                                                                                                                                      | UDP supports Broadcasting.                                                                                                                                                                                                                |
| Protocols                | TCP is used by HTTP, HTTPs, FTP, SMTP and Telnet.                                                                                                                                                                      | UDP is used by DNS, DHCP, TFTP, SNMP, RIP, and VoIP.                                                                                                                                                                                      |
| Stream Type              | The TCP connection is a byte stream.                                                                                                                                                                                   | UDP connection is message stream.                                                                                                                                                                                                         |
| Overhead                 | Low but higher than UDP.                                                                                                                                                                                               | Very low.                                                                                                                                                                                                                                 |

[More >>](https://www.geeksforgeeks.org/differences-between-tcp-and-udp/)

</details>
