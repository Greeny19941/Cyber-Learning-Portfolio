# TryHackMe - Linux Fundamentals Part 1/Windows Fundamentals 1

## 🐧 Linux Fundamentals 1 

### Key Learnings

- **echo** — outputs text to the terminal. Although straightforward, I wasn’t sure what its purpose would be in a working environment at first. After some reflection, I realised I’ve seen it used in scripts at work for logging or simple checks — which makes more sense now. Using **quotations** was also a helpful reminder for handling strings with spaces.  
- **whoami** — determines which user is currently logged in (similar to Windows). Simple, but useful for confirming user context when running commands or troubleshooting permissions.  
- **ls, cd, cat, pwd** — core navigation and file commands.  
  - *cat* = concatenate — new word for me, and a helpful one. It’s mainly used for displaying file contents or combining files, though I still need a bit more practice linking it conceptually to “concatenation” in programming.  
- Got stuck changing directories from `folder1` but figured out to use `cd ..` or `cd ~` to go up or return home. I had to search for help externally, which was a good reminder to check documentation first before getting stuck for too long.  

## Commands and Concepts

- **find** — searches entire directories efficiently, avoiding repetitive use of `ls` and `cd`.  
- **grep** — powerful for searching inside files; combining it with `-r` for recursive searches can save a lot of time when working with multiple files.  
- **Wildcards** like `*` — familiar from Windows, so this feels like a comfortable crossover point between systems.  
- **Shell operators** introduced new concepts:  
  - `&` — run a command in the background.  
  - `&&` — chain commands; only executes the next one if the previous succeeds.  
  - `>` — redirect output to a file (overwrite).  
  - `>>` — append output to a file.  

I hadn’t encountered most of these before, but they make sense logically and will be really useful when automating or chaining tasks in scripts.

## Reflection

There was a lot to absorb, especially around shell operators and file redirection. The logic behind the Linux command line is starting to feel clearer, but it’s definitely something that will require **regular practice** to build confidence.  

Overall, this was a strong introduction — it reminded me how transferable some of my existing IT knowledge is, while also showing how much more efficient Linux can be once you understand its structure and syntax.

## 🪟 Windows Fundamentals 1

### Key Learnings
I felt generally comfortable with this one given my experience with Windows, but I was introduced to a few new concepts such as **ADS (Alternate Data Streams)** — how files can contain more than one data stream within **NTFS**, and how some malware writers have used this to hide malicious data.  

I wasn’t previously aware of ADS since it doesn’t display to users by default, but I learned that **PowerShell** can be used to view it.  

Other commands and tools such as `%windir%` and `lusrmgr.msc` were already familiar from my work experience.  

### Reflection
This module reinforced knowledge I already had while introducing subtle but important Windows internals I hadn’t encountered before. It was a good reminder that even with familiar systems, there’s always something new to uncover — especially when it comes to **security implications**.
