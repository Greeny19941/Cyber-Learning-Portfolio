## 🧩 Active Directory Fundamentals

### Key Learnings
This was another room where much of the content has already been reinforced through my previous certifications and work experience. The benefits of **Active Directory (AD)** compared to standalone systems are well recognised, and terms like **OU** (Organisational Unit) and **AD DS** (Active Directory Domain Services) are already familiar to me.

- **Deleted objects protection** — common knowledge, though not something I encounter often day-to-day.  
- **Delegation of OUs** — not something I’ve personally managed before, but the room gave me confidence that I could handle it effectively in a real environment. Resetting Sophie’s password using another account was a practical exercise that solidified this understanding.  
- **PowerShell password reset** — possibly the first time I’ve done this via PowerShell. It’s a simple command but gives more scope for experimenting and understanding both administrative and security implications (attacking/defensive perspectives).

- *PowerShell scripts ran:
![download](https://github.com/user-attachments/assets/32d39ba3-8a80-4029-8296-04e3e8374757)

- *End result of password change and request to change at first log-on.
- ![download](https://github.com/user-attachments/assets/ca7d5dbb-2c85-45c6-a3ff-d0eb340b70fc)


### Group Policy & Domain Management
We created **OUs** and moved computers between them — something I already do at work — followed by group policy configuration.  
- Reminder that **Sysvol** is distributed over the network for Group Policy Objects (GPOs).  
- Created a GPO to:  
  - Restrict access to **Control Panel**  
  - Enforce **auto-lock after 300 seconds**  

I’ve done similar configuration work previously at Netbuilder, but this was a great hands-on refresher.

- *Group Policy Object, which was then linked to the Marketing OU (where our dummy user, Mark was present)
![download](https://github.com/user-attachments/assets/19d901d3-2080-4266-9f71-c2b9798ecb94)

-* When RDPing onto a VM, I tried to open Control Panel and was expectedly met with this error:
![download](https://github.com/user-attachments/assets/b35ad577-ce32-4f48-ab0f-80c0256f0d46)


### Kerberos & Authentication
The lab introduced **Kerberos**, which included terminology I hadn’t explored before, such as:  
- **KDC (Key Distribution Center)**  
- **TGT (Ticket Granting Ticket)**  
- **Session keys**  

While the jargon was initially dense, I gained a clearer understanding of how the domain controller authentication process works. The biggest takeaway: **passwords are never transmitted across the network in plain form**, thanks to hashing and encryption mechanisms.

### AD Structure & Terminology
Terminology was revisited to clarify concepts that had previously caused confusion:  
- **Trees** — multiple domains under one company (e.g., different departments). Requires **Enterprise Admins** for cross-domain management.  
- **Forests** — separate domains under different domain names (e.g., mergers or acquisitions). Requires **trust relationships** for resource access (e.g., file shares).  
  - By default, two-way trust relationships exist, but user authorisation across domains must still be explicitly configured.  

### Reflection
This room helped reinforce practical AD knowledge while expanding my understanding of **Kerberos authentication** and **domain trust models**. It also bridged theoretical understanding with hands-on application — from PowerShell password resets to GPO configuration — all of which align closely with both real-world administration and security perspectives.

