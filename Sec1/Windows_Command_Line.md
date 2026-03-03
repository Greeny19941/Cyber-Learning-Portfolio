# 🪟 Windows Command Line (TryHackMe)

## Basic System Information

- **systeminfo**, **ver** — familiar commands used to gather system details.  
- **driverquery | more** — new to me; I compared it with simply running `driverquery`. The `| more` pipe makes long outputs easier to read by displaying them one screen at a time — much more user-friendly for detailed results.  
- Also noted **winver**, which provides a GUI-based version window, complementing command-line output.

---

## Networking Commands

I’m already comfortable with common networking commands such as `ipconfig (/all)`, `ping`, `tracert`, `nslookup`, and `netstat`.  
However, I explored deeper options such as:  

- **netstat -a, -b, -o, -n** — expanded understanding of network connections and ports.  
  - **-o** shows process IDs.  
  - **-n** forces numerical IP and port display.  
- Combining these into `netstat -abon` gives a powerful, detailed view of open connections and associated processes.

---

## File & Disk Management

- **cd**, **dir** — core navigation commands I already use.  
  - `dir /a` — displays hidden/system files.  
  - `dir /s` — searches within the current directory and all subdirectories.  
- **tree** — a visually appealing way to view directory structures in the terminal; I prefer this slightly “graphical” view.  
- **mkdir**, **rmdir**, and `cd <directory>` are straightforward and remind me of their Linux equivalents — a nice crossover between systems.

---

## Process Management

- **tasklist** — known command but rarely used since Task Manager is more common in daily work.  
  - Used **tasklist /FI "imagename eq notepad.exe"** and learned that **eq** = “equal to,” **ne** = “not equal to.”  
- **taskkill** — useful for terminating processes by PID.  
- Overall, the Windows CLI feels quite powerful once you understand filters and switches.

---

## System Utilities and Other Commands

- **chkdsk**, **sfc /scannow** — familiar tools for disk and system integrity checks.  
- Learned that adding **/?** to any command displays built-in help — a great quick reference I’ll use more often.  
- **more** — helpful to paginate long outputs for better readability.  
- **shutdown -a** — new command to me, aborts a pending system shutdown (simple but very handy).

---

## Reflection

This room was largely a reinforcement of known concepts but introduced several practical enhancements I hadn’t explored before — particularly the use of **pipes**, **filters**, and advanced **netstat** options.  
It also highlighted how much crossover there is between Windows and Linux in the command-line world. I feel more confident in using the Windows CLI efficiently and plan to apply some of these commands more frequently in day-to-day troubleshooting and testing.
