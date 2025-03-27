User Datagram Protocol (UDP) is a **lightweight, connectionless transport protocol** that provides minimal services. 
Unlike TCP, UDP does **not require handshaking** before communication begins. It is commonly used in applications where **low latency and efficiency** are more critical than reliability.

### Key Characteristics:
- **Unreliable data transfer**: UDP does not guarantee delivery of data.
- **No ordering of messages**: Packets may arrive **out of order**.
- **No error recovery**: If a packet is lost or corrupted, it is **not retransmitted**.
- **Connectionless communication**: No need to establish or maintain a connection.
- **Low overhead**: Smaller header size compared to TCP (only 8 bytes).

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

### Reference Books
1. Kurose, J. F., & Ross, K. W. *Computer Networking: A Top-Down Approach*. Pearson.
2. Tanenbaum, A. S., & Wetherall, D. J. *Computer Networks*. Pearson.