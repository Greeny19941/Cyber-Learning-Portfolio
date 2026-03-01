# TryHackMe — SEC1 Intro Labs: Offensive Security Intro / Defensive Security Intro / Search Skills

## Section: Attack
### Tools & Commands Learned
- **`dirb`** – basic web directory brute-forcing to discover hidden pages.
- **`cat`** – viewing file contents on Linux.
- Refreshed knowledge of **`netstat`** (Windows vs Linux):
  - `netstat -a` – lists all active connections and listening ports.
  - `netstat -b` – shows the executable that created each connection (requires admin rights on Windows).

### Notes / Reflections
- Hands-on use of `dirb` was simple but valuable — first exposure to web enumeration using a tool.
- Linux commands like `cat` are fundamental but easy to overlook — good reinforcement from prior A+ studies.

---

## Section: Defence
### Concepts Introduced
- **CVE (Common Vulnerabilities and Exposures)** – encyclopaedia of known security vulnerabilities.  
  - Useful starting point when researching exploits; some details can be very technical.
- Awareness of active ports and executables is crucial for monitoring and defending systems.

---

## Section: Search & Recon / Social Media
### Browser Search Techniques
- **Exact phrase** `"..."` – returns pages with the exact text.  
- **`site:`** – restrict search to a specific domain.  
- **`-`** – exclude specific words or phrases.  
- **`filetype:`** – search for specific file types (e.g., `filetype:ppt cyber security` to find presentations).  

### Specialist Tools / Platforms
- **Shodan** – search for internet-connected devices running certain services.  
- **Censys** – searches for internet-connected systems, webcams, IoT, etc.  
- **VirusTotal** – checks suspicious files against multiple antivirus engines; community discussion can help filter false positives.  
- **HaveIBeenPwned** – checks if an email has appeared in known data breaches.  

### Notes / Reflections
- Browser search operators are **game-changing** — would have been invaluable during university research.  
- Social media awareness: even seemingly harmless public info can reveal sensitive details and affect security posture.  
- Shodan and Censys illustrate how exposed devices on the internet can be found and assessed — reinforces importance of defensive monitoring.

---

## 💡 Key Takeaways
- Hands-on tools like `dirb` and `cat` help develop practical lab skills.  
- Search operators and OSINT techniques dramatically enhance reconnaissance ability.  
- Awareness of public data, email breaches, and internet-connected devices is critical for both attack and defence mindsets.  
- Concepts like CVEs provide a structured starting point for vulnerability research.

---
