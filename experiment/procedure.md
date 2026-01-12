## Procedure for UDP Chat

- Send `PING` messages.
- On receiving the `PING`, the receiver sends a `PONG` message.
- There is chance of failure in message transmission.
- The aim is to receive a **3** `PONG` messages and fill in the number of `PING` messages required for this.