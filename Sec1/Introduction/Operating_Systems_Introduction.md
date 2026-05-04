# Operating Systems: Introduction – TryHackMe Write-Up

## Overview

This lab introduces the core concepts of operating systems (OS), focusing on how they interact with users, applications, and hardware. It reinforces foundational knowledge and highlights key responsibilities and security features of an OS.

---

## System Architecture

An operating system acts as an intermediary between:

- **User**
- **Applications**
- **Hardware**

It ensures that applications can run efficiently while managing system resources.

---

## Kernel Space vs User Space

A key concept revisited was the separation between:

- **Kernel Space**
  - Core part of the OS  
  - Has full access to hardware  
  - Handles critical system functions  

- **User Space**
  - Where applications run  
  - Restricted access to system resources  
  - Interacts with the kernel via system calls  

This separation is important for maintaining system stability and security.

---

## Core Responsibilities of an OS

The operating system is responsible for:

- **Process Management** – Managing running applications  
- **Memory Management** – Allocating and controlling RAM usage  
- **File System Management** – Handling file storage and access  
- **User Management** – Managing user accounts and permissions  
- **Device Management** – Controlling hardware components  

This lab reinforced that these responsibilities are standard across most operating systems.

---

## OS Security Features

Operating systems include built-in security mechanisms such as:

- **Authentication** – Verifying user identity  
- **Permissions** – Controlling access to resources  
- **Firewalls** – Filtering network traffic  
- **Process Isolation** – Preventing processes from interfering with each other  

These features help protect the system from unauthorised access and malicious activity.

---

## GUI vs CLI

The lab revisited the difference between:

- **GUI (Graphical User Interface)**  
  - User-friendly, visual interface  
  - Common in desktop environments  

- **CLI (Command Line Interface)**  
  - Text-based interface  
  - More efficient for advanced tasks  

This is relevant in environments such as Windows Server, where both options (Core and Desktop Experience) are available.

---

## Types of Operating Systems

Different operating systems are designed for specific purposes:

- **Desktop OS** – General user environments  
- **Server OS** – Designed for performance and uptime  
- **Mobile OS** – Optimised for portability and battery life  
- **Embedded OS** – Built into dedicated devices  
- **Virtual/Cloud OS** – Designed for scalable environments  

There is no “perfect” operating system—each is built to meet specific requirements.

---

## Key Takeaways

- Operating systems manage the interaction between hardware and software  
- Kernel space and user space separation is critical for security and stability  
- OS responsibilities are standardised across systems  
- Security features such as authentication and isolation are essential  
- Different OS types are designed for different use cases  

---

## SOC Relevance

Understanding operating systems is important for security roles because:

- Many attacks target OS-level vulnerabilities  
- Permissions and user management are key to access control  
- Logs and system behaviour are OS-dependent  
- Misconfigurations can lead to security weaknesses  

A strong understanding of OS fundamentals supports effective system analysis and incident investigation.

---

## Reflection

This lab reinforced existing knowledge from previous studies and practical experience. It provided a structured overview of operating system responsibilities and security features, which are essential for understanding how systems operate and how they can be secured.
