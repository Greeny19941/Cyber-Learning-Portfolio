# 🔐 Cryptography Basics (TryHackMe)

## Overview
This room provided an overview of cryptography and its importance in securing communication. While we rarely interact directly with cryptography in daily operations, it underpins the **CIA Triad** — ensuring confidentiality, integrity, and availability.

The room also introduced key industry standards and regulations such as **GDPR**, **PCI DSS**, and **HIPAA**, all of which reinforce the need for secure handling of data. I’ve been exposed to these previously through certifications and training, but this served as a good refresher of their connection to encryption and compliance.

---

## Key Learnings

### Plaintext, Ciphertext, and the Encryption Process
We revisited how plaintext becomes ciphertext and vice versa through encryption and decryption. It was a clear demonstration of the flow of data security in motion.

---

### Historical Ciphers
It was fascinating to see cryptography’s origins traced back to **ancient Egypt**, long before the digital era. The **Caesar cipher** example showed how letters were shifted by a fixed number (e.g., A→D with a shift of 3).  
Although primitive by modern standards, it was interesting to realise that **the principles of obfuscation and key-based substitution are ancient concepts**, simply modernised through computing.

---

### Symmetric vs Asymmetric Encryption
This section reinforced topics covered in **ISC² CC**:
- **Symmetric encryption:** uses a single shared key for encryption and decryption.  
- **Asymmetric encryption:** uses a **public** and **private** key pair.  

We also touched on historical and modern standards:
- **DES** — first widely used standard; later broken by brute force in under 24 hours.  
- **3DES** — a temporary fix; deprecated in 2019 but still used in legacy systems.  
- **AES (Advanced Encryption Standard)** — the current standard since 2001.  

> In general, the higher the bit length, the stronger the encryption — as it increases the computational time required to break it.

---

### Mathematical Operations: XOR and Modulo
The **XOR (exclusive OR)** operation was challenging to grasp conceptually. It’s a binary operation used in cryptographic algorithms for key mixing and bitwise comparison.  
I found the **Modulo operator** easier to understand once I realised it focuses on the **remainder** after division, not the quotient.  

I used [WolframAlpha Modulo Calculator](https://www.wolframalpha.com/input?i=modulo) to verify my calculations, which helped solidify my understanding of how modulo works in encryption mathematics.

Although I found these operations complex at first, I now appreciate how mathematical unpredictability is a fundamental component of cryptography — it’s *meant* to be complicated!

---

## Reflection
This room helped me connect high-level encryption concepts (AES, keys, and ciphers) with the underlying mathematics that makes them secure.  
The history and evolution from **Caesar ciphers** to **AES** made the topic more approachable, and while some of the binary math took time to digest, it clarified why cryptography is such a specialised field — it blends logic, math, and security principles seamlessly.
