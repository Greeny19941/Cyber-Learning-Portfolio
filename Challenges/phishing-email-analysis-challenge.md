# TryHackMe – Phishing Email Analysis Challenge

## Overview
This challenge involved analysing a series of 10 simulated emails under timed conditions (30 seconds per email) and classifying each as legitimate or phishing-based, with justification required for each decision.

## Outcome
- Completed with high accuracy
- No lives lost during the challenge
- Demonstrated consistent identification of phishing indicators under time pressure
![Phishing Challenge](Screenshots/phishingchallenge.png)

## Key Phishing Indicators Identified

### 1. Character Substitution / Homoglyph Attacks
Detected attempts to impersonate legitimate domains using character substitution (e.g. "rn" used to mimic "m") to deceive visual scanning.

### 2. Urgency and Pressure Tactics
Emails frequently used urgent language to induce fast, emotional decision-making rather than rational review.

### 3. Sender Analysis
Checked sender addresses for:
- Domain inconsistencies
- Spoofed display names
- Mismatched reply-to fields

### 4. Links and Attachments
Flagged suspicious:
- Unexpected attachments
- Mismatched or obfuscated URLs
- Non-business-relevant file types

## Methodology
Each email was assessed under time pressure using a structured mental checklist:
1. Verify sender legitimacy  
2. Scan for linguistic manipulation (urgency, fear, authority)  
3. Inspect links and attachments  
4. Identify visual spoofing techniques  
5. Classify and justify decision

## Real-World Application
This challenge reinforced practical skills used in a sandboxed security environment during previous work with the Security team at Emeria, where email headers and message content were analysed in isolated environments for threat identification.

## Key Takeaways
- Phishing attacks rely heavily on psychological manipulation rather than technical complexity
- Small visual tricks (e.g. homoglyphs) are highly effective against untrained users
- Structured, repeatable analysis significantly improves detection accuracy under time pressure
