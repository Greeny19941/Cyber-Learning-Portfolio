# How Websites Work – TryHackMe Write-Up

## Overview

This lab introduces the fundamental components of how websites operate, focusing on the interaction between the front-end and back-end. It also explores core web technologies and highlights basic security considerations.

---

## Front-End vs Back-End

Websites consist of two main components:

- **Front-End**
  - The part users interact with in a browser
  - Built using HTML, CSS, and JavaScript

- **Back-End**
  - Handles server-side logic, databases, and processing
  - Communicates with the front-end over the internet

---

## Core Web Technologies

### HTML (HyperText Markup Language)
- Defines the structure of a webpage
- Key elements include:
  - `<!DOCTYPE html>`
  - `<body>`

---

### CSS (Cascading Style Sheets)
- Controls the visual styling of a webpage

---

### JavaScript
- Adds interactivity and dynamic behaviour
- Can be used inline or via external files

---

## Sensitive Data Exposure

Sensitive data exposure is a significant security risk in web applications.

Examples include:
- Credentials left in source code
- API keys or tokens exposed to users
- Data transmitted in clear text
- Hidden links or sensitive information visible in page source

It is good practice to:
- Inspect page source code
- Identify exposed credentials
- Look for suspicious or hidden content

---

## HTML Injection

HTML Injection occurs when user input is not properly validated or sanitised.

Key points:
- Similar to other injection attacks (e.g. SQL injection)
- Exploits poor input validation
- Can lead to data exposure or manipulation

Mitigation:
- Validate and sanitise input
- Encode output properly

---

## Key Takeaways

- Websites rely on front-end and back-end interaction
- HTML, CSS, and JavaScript form the foundation of web applications
- Sensitive data exposure is a common vulnerability
- Injection attacks highlight the importance of input validation

---

## SOC Relevance

Understanding how websites work is important because:

- Many attacks target web applications
- Page source can reveal exposed data or misconfigurations
- Injection vulnerabilities are commonly exploited
- Analysts investigate suspicious web traffic regularly

Many web-based attacks rely on manipulating client-server interactions, making an understanding of front-end and back-end behaviour essential for detection and analysis.

---

## Reflection

This lab reinforced foundational web concepts while introducing important security considerations. It highlighted how poor input handling and exposed data can lead to vulnerabilities.
