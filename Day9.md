# Day 9 - Networking Fundamentals

**Date:** 2024-08-03

## Summary
Today, I focused on networking fundamentals, including Ethernet cables, UTP vs. fiber optics, and the OSI and TCP/IP models.

## Detailed Notes

### Networking Fundamentals
I completed two videos on networking and learned about the following topics:

#### Ethernet Cables
- **Ethernet Cables:**
  - Ethernet cables are used to connect devices within a local area network (LAN).
  - They come in various categories, such as Cat5, Cat5e, Cat6, Cat6a, Cat7, and Cat8, each supporting different speeds and distances.

#### UTP vs. Fiber Optics
- **Unshielded Twisted Pair (UTP):**
  - Commonly used for most networking purposes.
  - Consists of pairs of wires twisted together to reduce interference.
  - Suitable for short to medium distances.
  
- **Fiber Optics:**
  - Uses light to transmit data, offering higher speeds and longer distances compared to UTP.
  - Less susceptible to electromagnetic interference.
  - Ideal for backbone connections and long-distance communication.

#### OSI and TCP/IP Models
- **OSI Model:**
  - A conceptual framework used to understand network interactions in seven layers:
    1. **Physical Layer:** Deals with the physical connection between devices and the transmission of binary data.
    2. **Data Link Layer:** Handles error detection and correction from the physical layer and manages how data is placed on the network medium.
    3. **Network Layer:** Manages logical addressing and routing of data packets.
    4. **Transport Layer:** Ensures data is transferred reliably and without errors.
    5. **Session Layer:** Manages sessions or connections between applications.
    6. **Presentation Layer:** Translates data between the application layer and the network format.
    7. **Application Layer:** Closest to the end user, providing network services directly to applications.

- **TCP/IP Model:**
  - A more simplified, four-layer model used to understand network interactions:
    1. **Link Layer (Network Interface):** Combines the physical and data link layers of the OSI model.
    2. **Internet Layer:** Equivalent to the network layer in the OSI model, handling logical addressing and routing.
    3. **Transport Layer:** Corresponds to the transport layer in the OSI model, ensuring data transfer reliability.
    4. **Application Layer:** Combines the OSI model's session, presentation, and application layers, providing network services to applications.

#### OSI vs TCP/IP

| OSI Model        | TCP/IP Model  |
| ---------------- | ------------- |
| Application      |               |
| Presentation     | Application   |       
| Session          |               |
| ---------------- | ------------- |     
| Transport        | Transport     |
| Network          | Internet      |
| ---------------- | ------------- |
| Data Link Layer  |               |
| Physical         | Link Layer    |