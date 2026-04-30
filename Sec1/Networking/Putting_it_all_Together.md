# Putting It All Together – TryHackMe Write-Up

## Overview

This lab brings together previously covered concepts to explain how websites operate as a complete system. It introduces supporting infrastructure, server technologies, and the distinction between static and dynamic content.

---

## Web Infrastructure Components

Several key components that support modern web applications were introduced:

- **Load Balancers**  
  - Distribute traffic across multiple servers  
  - Improve performance and reliability  

- **Web Application Firewalls (WAFs)**  
  - Filter and monitor HTTP traffic  
  - Help protect against common web attacks  

- **Content Delivery Networks (CDNs)**  
  - Cache content across multiple geographic locations  
  - Improve load times and reduce server load  

These components are commonly used in production environments to ensure availability, performance, and security.

---

## Web Server Software

The lab introduced common web server technologies:

- **Apache**  
- **Nginx**  
- **Node.js**

These handle incoming HTTP requests and serve content to users.

Although familiar by name, this clarified their role as the systems responsible for delivering web content and managing traffic between clients and servers.

---

## Virtual Hosts

A key concept introduced was **virtual hosting**:

- Multiple websites can run on a single server  
- Each site is identified by its domain name  
- The server uses HTTP headers (such as the Host header) to determine which site to serve  

This corrected a misconception that each website requires a separate server.

---

## Static vs Dynamic Content

Websites can serve two types of content:

### Static Content
- Does not change  
- Examples: HTML, CSS, images  

### Dynamic Content
- Generated in real-time by the server  
- Examples:
  - Blog feeds  
  - Dashboards  
  - Weather widgets  

Dynamic content is processed on the back-end, meaning the client only sees the final rendered output—not the underlying logic.

---

## Scripting and Back-End Languages

The lab briefly introduced back-end scripting languages:

- Python  
- Ruby  
- Perl  
- PHP  

These are used to:
- Process user input  
- Interact with databases  
- Call external services  

Back-end code is not visible to the client, as it runs on the server before the response is sent.

---

## Key Takeaways

- Modern websites rely on multiple infrastructure components  
- Web servers handle requests and deliver content  
- Virtual hosting allows multiple websites to share a single server  
- Dynamic content is generated on the server and not visible in source code  
- Back-end languages drive application logic and data processing  

---

## SOC Relevance

Understanding how web infrastructure operates is important because:

- Load balancers and CDNs can affect how traffic appears in logs  
- WAFs play a key role in detecting and blocking malicious requests  
- Virtual hosting can complicate investigations when multiple domains share infrastructure  
- Dynamic applications introduce more attack surface compared to static sites  

This knowledge helps analysts better interpret web traffic and identify abnormal behaviour.

---

## Reflection

This lab consolidated previous knowledge and clarified how different components interact within a web environment. It reinforced the importance of understanding both infrastructure and application behaviour when analysing web-based systems.
