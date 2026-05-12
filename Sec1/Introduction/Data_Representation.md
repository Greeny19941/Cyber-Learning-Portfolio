# Data Representation

## Overview

This room introduces the concept of **data representation in computing**, focusing on how computers encode information such as colours using **binary, decimal, and hexadecimal systems**.

Computers fundamentally operate using binary, meaning everything is represented using only two values: **0 and 1**.

---

## Binary and Colour Representation

Binary was previously introduced in the context of subnetting, but in this lab it is applied to **colour encoding**.

Using 3 binary bits, we can represent:

- 2^3 = 8 possible combinations (colours)

Each bit represents an RGB (Red, Green, Blue) channel being either ON or OFF:

| Binary | Colour |
|--------|--------|
| 000    | Black  |
| 001    | Blue   |
| 010    | Green  |
| 100    | Red    |

This system is very limited in terms of colour depth.

---

## Expanding Colour Depth

To represent more realistic and detailed colours, more bits are required.

Using 8 bits per channel (RGB):

- 256^3 = 16,777,216 possible colours  
- This allows for “true colour” representation used in modern displays

---

## Hexadecimal Representation

Binary is efficient for machines but difficult for humans to read. This is where hexadecimal comes in.

Hexadecimal:

- Base 16 system (0–15)
- Uses digits 0–9 and letters A–F

| Decimal | Hex |
|--------|-----|
| 10     | A   |
| 11     | B   |
| 12     | C   |
| 13     | D   |
| 14     | E   |
| 15     | F   |

Example:
- Binary: `0110`
- Decimal: `6`
- Hex: `6`

Hex makes large binary values much easier to read and work with.

---

## Key Takeaways

- Computers use binary (0 and 1) to represent all data
- Small binary values can represent basic colours (e.g. 8 colours using 3 bits)
- Modern colour systems use 24-bit colour (16.7 million colours)
- Hexadecimal simplifies binary representation for humans
- RGB values are commonly expressed in hex in computing and web design

---

## Summary

This lab helped reinforce how binary can extend beyond networking and be used to represent visual data such as colour. It also highlighted why hexadecimal is widely used as a human-friendly shorthand for binary data.
