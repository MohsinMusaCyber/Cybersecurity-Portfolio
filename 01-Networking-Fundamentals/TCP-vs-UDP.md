# TCP vs UDP

## Overview

TCP (Transmission Control Protocol) and UDP (User Datagram Protocol) are two of the most important transport layer protocols used on modern networks.

---

# TCP

TCP is a connection-oriented protocol.

Before any data is sent, a connection is established using the Three-Way Handshake.

### Advantages

- Reliable delivery
- Error checking
- Packet ordering
- Flow control
- Retransmission of lost packets

### Common Uses

- Web browsing (HTTPS)
- Email
- File transfers (FTP)
- Remote administration (SSH)

---

# UDP

UDP is a connectionless protocol.

It sends data without establishing a connection first, making it much faster than TCP.

### Advantages

- Very fast
- Low latency
- Minimal overhead

### Disadvantages

- No guarantee of delivery
- No packet ordering
- No retransmission

### Common Uses

- Video streaming
- Voice over IP (VoIP)
- Online gaming
- DNS

---

# TCP vs UDP

| TCP | UDP |
|------|------|
| Connection-oriented | Connectionless |
| Reliable | Best effort |
| Slower | Faster |
| Error checking | Minimal checking |
| Ordered packets | No packet ordering |
| Higher overhead | Low overhead |

---

## What I Learned

Understanding the differences between TCP and UDP helps explain why different applications choose different protocols depending on whether reliability or speed is more important.

---

*Created as part of my Cybersecurity Portfolio.*
