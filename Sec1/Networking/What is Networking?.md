# What is Networking? 

## Overview

This lab introduces the fundamental concept of networking. While the content is very beginner-focused, it serves as a useful refresher of core principles that underpin more advanced cybersecurity topics.

The lab begins by defining what a network is. Importantly, it highlights that networks are not limited to IT systems—they can also refer to real-world systems such as power grids or postal networks. In computing, a network simply refers to interconnected devices that can communicate with one another.

The internet itself is introduced as the largest example of a network: a global system connecting millions of smaller networks.

Having already completed the CompTIA Network+ certification, most of this lab revisited familiar concepts, but it provided a useful recap of key fundamentals.

---

## Public vs Private Networks

The distinction between public and private networks was covered:

- **Public networks**: Accessible over the internet (e.g. websites, cloud services)  
- **Private networks**: Internal networks (e.g. home or corporate LANs)  

Understanding this distinction is essential in cybersecurity, particularly when considering attack surfaces and exposure.

---

## IP Addressing

The lab introduces basic IP addressing concepts:

- IPv4 addresses are **32-bit**, split into **4 octets**  
- Each device on a network must have a **unique IP address**  
- A single IP address cannot be used by multiple devices simultaneously within the same network  

It also touches on **IP exhaustion**, a known limitation of IPv4 due to its finite address space (~4.3 billion addresses).

### IPv6

To address IPv4 limitations, IPv6 was introduced:

- **128-bit addressing**  
- Vastly larger address space (effectively eliminating exhaustion concerns)  

Although IPv6 adoption is increasing, IPv4 is still widely used in practice.

---

## MAC Addresses

The lab explains how **MAC (Media Access Control) addresses** uniquely identify network interfaces:

- First **6 characters**: Vendor/manufacturer identifier (OUI)  
- Last **6 characters**: Unique device identifier  

A key security takeaway is that MAC addresses can be **spoofed**, meaning an attacker can impersonate another device on the network. This was demonstrated in the associated task, reinforcing how easily identity can be manipulated at a network level.

---

## ICMP and Ping

The lab concludes with a recap of the `ping` command:

- Uses the **Internet Control Message Protocol (ICMP)**  
- Tests connectivity between devices  
- Measures latency and reliability  

This is a simple but essential tool for:
- Troubleshooting network issues  
- Verifying connectivity  
- Basic network reconnaissance  

---

## Key Takeaways

- Networking concepts extend beyond IT and apply to many real-world systems  
- The internet is a large-scale network of interconnected smaller networks  
- IPv4 limitations led to the development of IPv6  
- MAC address spoofing highlights a basic but important security weakness  
- ICMP and ping remain fundamental tools for network diagnostics  

---

## Reflection

Although this lab is aimed at beginners, it served as a useful refresher of core networking principles. With a background in Network+, the content was familiar, but it reinforces the foundational knowledge required for more advanced topics such as network security, enumeration, and traffic analysis.

For a cybersecurity learner, mastering these basics is essential before progressing into more complex attack and defence techniques.
