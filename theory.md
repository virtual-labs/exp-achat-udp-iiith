## What is UDP ?

User Datagram Protocol (UDP) is a **lightweight, connectionless transport protocol** that provides minimal services. 
Unlike TCP, UDP does **not require handshaking** before communication begins. It is commonly used in applications where **low latency and efficiency** are more critical than reliability.

---

### UDP Packet Creation and Transmission

* UDP does **not require a handshake** before communication begins, unlike TCP.
* When an application sends data, UDP creates a packet called a **datagram**.
* This datagram includes a fixed **8-byte header** and the data payload.
* The header contains essential information such as the source and destination port numbers.
* UDP sends this datagram directly to the destination IP address without any confirmation from the receiver.

***

### Unreliable and Connectionless Nature

* **Datagrams are independent units** and may arrive out of order, or not at all.
* UDP does **not have built-in error recovery**. If a packet is lost or corrupted, it is not retransmitted.
* This lack of guaranteed delivery and retransmission is why UDP is considered an **unreliable protocol**.
* UDP communication is **connectionless**, meaning it doesn't establish or maintain a connection. This reduces overhead and delay, which is ideal for time-sensitive applications.
* If reliability is a requirement, the application must handle packet loss and retransmission on its own.

---

### Key Characteristics:
- **Unreliable data transfer**: UDP does not guarantee delivery of data.
- **No ordering of messages**: Packets may arrive **out of order**.
- **No error recovery**: If a packet is lost or corrupted, it is **not retransmitted**.
- **Connectionless communication**: No need to establish or maintain a connection.
- **Low overhead**: Smaller header size compared to TCP (TCP header ranges from 20-60 bytes as compared to UDP header has fixed size of 8 bytes).

## Use Cases of UDP
UDP is useful for applications that **prioritize speed over reliability**:

- **Finer application-level control**: Allows applications to manage packet loss, retransmission, and congestion control.
- **No connection establishment**: Reduces delay, making it suitable for time-sensitive applications.
- **No connection state**: Ideal for handling large numbers of clients efficiently.
- **Small packet header overhead**: More efficient for simple data transmission.

### Common Applications:
1. **Streaming Media (Audio/Video)**
2. **DNS (Domain Name System)**
3. **Online Gaming**
4. **IoT (Internet of Things) Devices**