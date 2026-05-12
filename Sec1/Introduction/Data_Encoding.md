# Data Encoding – TryHackMe Write-Up

## Overview

This lab introduces the concept of data encoding and explains how computers represent characters and languages digitally. It highlights the challenges of maintaining consistency across different systems and the evolution from ASCII to Unicode standards.

Although familiar with encoding issues from troubleshooting scenarios, this lab provided a clearer understanding of why encoding mismatches occur.

---

## What is Data Encoding?

Data encoding allows computers to represent characters, symbols, and text in a standardised digital format.

For communication to work correctly:
- Both systems must interpret characters using the same encoding standard
- A character such as `T` should map to the same binary value across systems

Encoding issues occur when different standards or character sets are used.

---

## ASCII

The lab introduced **ASCII (American Standard Code for Information Interchange)**:

- A 7-bit character encoding standard
- Originally designed for English characters and symbols

ASCII supports:
- Uppercase letters
- Lowercase letters
- Numbers
- Basic symbols

Additional “patches” and extensions were later introduced to support more characters, such as the euro symbol (`€`).

However, different systems implemented different extensions, which led to compatibility problems and inconsistent outputs.

---

## Language Complexity

The lab highlighted how languages increase encoding complexity.

Languages such as:
- Japanese
- Chinese
- Arabic

require significantly more characters than English.

English primarily relies on:
- 26 uppercase letters
- 26 lowercase letters

Whereas other languages may require thousands of unique symbols or characters.

---

## Unicode

To address these limitations, **Unicode** was developed.

Unicode:
- Standardises character representation globally
- Supports approximately 157,000 characters
- Includes thousands of emoji sequences

This removes the need to choose separate encoding systems for different languages.

---

## UTF Standards

The lab briefly introduced common Unicode encoding formats:

- **UTF-8**
  - Most commonly used on the web
  - Efficient for English text
  - Variable length encoding

- **UTF-16**
  - Uses 2 or more bytes per character

- **UTF-32**
  - Uses 4 bytes per character
  - Simpler structure but less storage efficient

UTF-8 is widely adopted because it balances compatibility and efficiency.

---

## Practical Understanding

Although largely theoretical, the lab helped explain encoding-related issues commonly encountered during troubleshooting, such as:

- Garbled characters
- Incorrect symbol display
- Compatibility problems between systems

---

## Key Takeaways

- Encoding allows computers to represent text and symbols consistently
- ASCII was limited in scope and primarily designed for English
- Unicode standardised character representation globally
- UTF-8 is the dominant encoding format used on the web
- Different encoding standards can cause compatibility issues

---

## SOC Relevance

Understanding data encoding is useful in cybersecurity because:

- Encoded data appears frequently in logs, scripts, and malware analysis
- Attackers may use encoding to obfuscate malicious content
- Analysts often encounter encoded strings during investigations
- Correct interpretation of data is essential for forensic and incident response work

Encoding knowledge also assists with troubleshooting corrupted or misinterpreted data.

---

## Reflection

This lab clarified the purpose and evolution of character encoding standards. While theoretical, it provided useful context for understanding real-world compatibility issues and how modern systems handle multilingual communication.
