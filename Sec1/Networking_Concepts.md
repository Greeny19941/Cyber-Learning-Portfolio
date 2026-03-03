# 🌐 Networking Concepts (TryHackMe)

## Overview
This was a very useful room, particularly as I plan to begin studying for **CompTIA Network+** after my holiday. It served as a great head start and refresher of key networking principles, some of which I had already covered in the **ISC² Certified in Cybersecurity (CC)** exam.

---

## Key Learnings

### OSI Model
- The mnemonic **“Please Do Not Throw Spinach Pizza Away”** remains a memorable way to recall the OSI model’s seven layers.  
- The concept of **decapsulation** was demonstrated well — showing how data moves *down* the OSI stack when sent and *up* the stack when received.

### TCP/IP Model
- Reviewed the **TCP/IP model**, which simplifies the OSI model by merging certain layers:  
  - Layers 5, 6, and 7 (Application, Presentation, Session) → **Application Layer**  
  - Layers 1 and 2 (Physical, Data Link) → **Link Layer**  
- The TCP/IP model’s condensed structure helped clarify how real-world protocols map to each layer.

### Subnetting
- Subnetting was clearly explained using the **255.255.255.0** mask, which equates to **/24**.  
- The leftmost 24 bits represent the *network portion*, while the last octet represents the *host range*.  
- I understand the concept but recognise subnetting may be an area I’ll need to study more deeply for the Network+ exam.  
- Refreshed knowledge of **private IP ranges**, which I’ll aim to memorise as part of my upcoming studies.

### TCP vs UDP
- Revisited **UDP** vs **TCP**, reinforcing:  
  - **TCP** = connection-oriented, reliable delivery using the **SYN-ACK handshake**.  
  - **UDP** = faster, connectionless protocol used where reliability is less critical.  
- The technical flow — segments, frames, and encapsulation — still needs more study for full confidence, but I expect **Network+** will help solidify this understanding.

---

## Reflection
Overall, this room provided a solid warm-up for **Network+**, reinforcing familiar topics while clarifying a few gaps. Subnetting and packet flow remain priority areas to practise, but I feel much more confident revisiting networking theory with this practical foundation in place.
