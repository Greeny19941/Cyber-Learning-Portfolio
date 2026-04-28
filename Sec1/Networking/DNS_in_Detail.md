# DNS in Detail 

## Overview

This lab explores the Domain Name System (DNS), which is responsible for translating human-readable domain names into IP addresses (and vice versa). While this was largely a refresher from prior study, it reinforced key concepts and introduced some useful details around domain structure and DNS records.

DNS is a critical component of both networking and cybersecurity, as it underpins how systems locate and communicate with each other across the internet.

---

## Domain Structure

DNS follows a hierarchical structure:

- **Root Domain** (.)
- **Top-Level Domain (TLD)** – e.g. `.com`, `.org`, `.co.uk`
- **Second-Level Domain** – e.g. `google` in `google.com`
- **Subdomains** – e.g. `mail.google.com`

### Types of TLDs

- **gTLD (Generic Top-Level Domains)** – e.g. `.com`, `.net`, `.org`
- **ccTLD (Country Code Top-Level Domains)** – e.g. `.uk`, `.fr`, `.jp`

### Key Limits

- Maximum length of a **domain name**: 253 characters  
- Maximum length of a **subdomain label**: 63 characters  

These constraints were new to me and are useful to understand when working with DNS configurations or automation.

---

## DNS Record Types

The lab covered several common DNS record types:

- **A Record** – Maps a domain to an IPv4 address  
- **AAAA Record** – Maps a domain to an IPv6 address  
- **CNAME Record** – Maps one domain to another (alias)  
- **MX Record** – Specifies mail servers for a domain  
- **TXT Record** – Stores arbitrary text (often used for verification, SPF, DKIM)  

Understanding these records is essential for both system administration and security analysis.

---

## DNS Resolution Process

The lab demonstrated how DNS queries are resolved:

1. A request is made to a **recursive DNS resolver**
2. The resolver queries:
   - **Root servers**
   - **TLD servers**
   - **Authoritative DNS servers**
3. The authoritative server returns the final answer

- **Recursive resolver**: Performs the “search” for the answer  
- **Authoritative server**: Holds the definitive DNS records  

### Caching and TTL

To improve efficiency, DNS responses are cached:

- **TTL (Time To Live)** determines how long a record is stored in cache  
- Reduces repeated queries and improves performance  

---

## Practical Commands

The lab included a guided demonstration of querying DNS records from the command line.

### Example:

```bash
nslookup --type=TXT website.thm
