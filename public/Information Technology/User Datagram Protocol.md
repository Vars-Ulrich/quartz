---
aliases:
  - UDP
---
> In computer networking, the **User Datagram Protocol** (UDP) is one of the core communication protocols of the Internet protocol suite used to send messages (transported as datagrams in packets) to other hosts on an [[Internet Protocol]] (IP) network. Within an IP network, UDP does not require prior communication to set up communication channels or data paths.
>
> UDP uses a simple connectionless communication model with a minimum of protocol mechanisms. UDP provides checksums for data integrity, and port numbers for addressing different functions at the source and destination of the datagram. It has no handshaking dialogues and thus exposes the user's program to any unreliability of the underlying network; there is no guarantee of delivery, ordering, or duplicate protection. If error-correction facilities are needed at the network interface level, an application may instead use [[Transmission Control Protocol|Transmission Control Protocol (TCP)]] or [[Stream Control Transmission Protocol|Stream Control Transmission Protocol (SCTP)]] which are designed for this purpose.
>
> UDP is suitable for purposes where error checking and correction are either not necessary or are performed in the application; UDP avoids the overhead of such processing in the protocol stack. Time-sensitive applications often use UDP because dropping packets is preferable to waiting for packets delayed due to retransmission, which may not be an option in a real-time system.
>
> The protocol was designed by David P. Reed in 1980 and formally defined in RFC 768.
>
> [Wikipedia](https://en.wikipedia.org/wiki/User%20Datagram%20Protocol)