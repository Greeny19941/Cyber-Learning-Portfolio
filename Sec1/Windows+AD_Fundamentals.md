## 🪟 Windows Fundamentals 1

### Key Learnings
I felt generally comfortable with this one given my experience with Windows, but I was introduced to a new concept called **ADS (Alternate Data Streams)** — how files can contain more than one data stream within **NTFS**, and how some malware writers have used this to hide malicious data.  

I wasn’t previously aware of ADS since it doesn’t display to users by default, but I learned that **PowerShell** can be used to view it.  

Other commands and tools such as `%windir%` and `lusrmgr.msc` were already familiar from my work experience.  

### Reflection
This module reinforced knowledge I already had while introducing subtle but important Windows internals I hadn’t encountered before. It was a good reminder that even with familiar systems, there’s always something new to uncover — especially when it comes to **security implications**.


## 🪟 Windows Fundamentals Part 2

### Key Learnings
This lab expanded on familiar Windows tools and introduced a few new insights that I hadn’t fully explored before.  

- **System Configuration (msconfig)** — mostly familiar, but this reinforced that it’s used for managing startup applications and boot settings. I also learned about using **shell:startup** for managing startup apps on Windows Server OSs, though I have used this utility before.  
- Explored the **Tools** tab in System Configuration — an area I rarely visit — and found it helpful for accessing administrative utilities directly.  
- The lab focused heavily on **command-line alternatives** for common GUI tools. While I’m likely to continue using the GUI for ease of use, it’s good to know the command equivalents for efficiency and scripting.  

### Commands and Concepts
- **Virtual Memory** — revisited the concept of allocating additional virtual memory when physical RAM is full (previously covered in CompTIA A+).  
- **Startup and Recovery** — learned to configure the system to write debugging information on BSOD errors, rather than relying solely on Event Viewer.  
- **Computer Management** — covered key components:  
  - Task Manager  
  - Event Viewer  
  - Shared Folders  
  - Performance Monitor  
  - Device Manager  
  - Disk Management  
  - Services and Applications  
- **Services** — reviewed service startup types (Automatic, Manual, Disabled). I regularly use this when restarting local services such as the **Print Spooler**.  
- **System Information (msinfo32)** — useful for gathering detailed system specifications.  
- **Resource Monitor** — rarely used in my workflow, but valuable for monitoring CPU, memory, and disk usage during troubleshooting.  
- **Command Line** — discovered the **cls** command to clear the terminal (something I never knew before). Other commands like `hostname`, `whoami`, `ipconfig`, and `netstat` were already familiar.  
- **Registry Editor (regedit)** — brief overview, though I’ve used this tool many times before for troubleshooting and configuration changes.  

### Reflection
This lab was more in-depth than **Windows Fundamentals 1**, but still within my comfort zone. It provided useful reinforcement of Windows internals and introduced command-line alternatives to common GUI operations — something I’d like to explore further for efficiency.  

Overall, it felt like a strong continuation of the fundamentals, reinforcing both **system administration awareness** and **troubleshooting skills** I use regularly in my IT support role.


## 🪟 Windows Fundamentals 3

### Key Learnings

- **Windows Updates**  
  - Revisited Patch Tuesdays (typically the 2nd week of each month).  
  - Reinforced the importance of keeping systems patched regularly.

- **Windows Security / Virus & Threat Protection**  
  - Controlled Folder Access: protects certain files/folders from unauthorized apps.  
  - Adding exclusions in Windows Defender Firewall can reduce false positives.  

- **Windows Defender Firewall**  
  - Recommended to keep enabled.  
  - Command to open: `WF.msc`.  
  - Used for enabling/disabling apps or features securely.

- **Microsoft Defender SmartScreen**  
  - Protects against malware, phishing, and untrusted applications.  
  - Found in *App & Browser Control* settings.  
  - Keeping default exploit protection is advised unless fully confident.

- **Device Security**  
  - Core Isolation & Memory Integrity: virtualisation-based protections.  
  - Usually left on; changing requires 100% confidence.  
  - TPM (Trusted Platform Module) supports BitLocker drive encryption.  

- **Volume Shadow Copy Service (VSS)**  
  - Creates system restore points (System Restore).  
  - Useful for recovery after malware attacks, though some malware tries to disable/delete them.  
  - Conceptually overlaps with practices covered in CompTIA A+ Core 1 and ISC² CC.  

---

### Commands / Concepts

| Feature | Command / Path | Notes |
|---------|----------------|-------|
| Windows Defender Firewall | `WF.msc` | Enables/disables firewall apps and features |
| Core Isolation / Memory Integrity | Device Security → Core Isolation | Recommended to leave on default |
| TPM / BitLocker | BitLocker Management | Encrypt full drives, works with TPM |
| System Restore / VSS | Control Panel → System → System Protection | Used to create or restore restore points |

---

### Reflection

This lab reinforced **security-first thinking** in Windows environments.  
Many of the concepts (TPM, BitLocker, System Restore) were familiar, but TryHackMe emphasized **realistic threat scenarios**, such as malware targeting VSS or protected folders.  

Key takeaways:  
- Always keep **default security settings** unless fully confident.  
- Understand the tools and their purposes, even if you rarely interact with them.  
- Hands-on exposure (controlled folder access, firewall rules, SmartScreen) is invaluable for bridging theoretical knowledge with practical application. 
