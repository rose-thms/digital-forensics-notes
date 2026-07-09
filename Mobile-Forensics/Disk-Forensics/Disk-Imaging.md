# Disk Imaging in Digital Forensics

## Overview

Disk imaging is the process of creating an exact forensic copy of a storage device while preserving the integrity of the original evidence.

A forensic image contains the complete contents of a storage device, including:
- Active files
- Deleted files
- File system structures
- Metadata
- Unallocated space

---

# Forensic Imaging Process

The standard forensic acquisition workflow:

1. Identify the storage media
2. Connect the device using a write blocker
3. Create a forensic image
4. Calculate hash values
5. Verify image integrity
6. Analyze the acquired image

---

# Image vs Clone

## Forensic Image

A forensic image is a bit-by-bit copy of a storage device stored as an evidence file.

Examples:
- E01
- RAW/DD
- AFF

Advantages:
- Maintains evidence integrity
- Contains metadata
- Can be verified using hashes

---

## Clone

A clone is an exact copy directly written to another storage device.

Example:

Source Drive → Destination Drive

Advantages:
- Useful for hardware replacement
- Direct duplicate

Limitations:
- Less forensic metadata
- Not usually used as the primary evidence format

---

# Write Blockers

A write blocker prevents any modification to the original evidence during acquisition.

Types:

## Hardware Write Blocker

Physical device placed between the evidence drive and forensic workstation.

Examples:
- Tableau Write Blocker
- OpenText TD2U

## Software Write Blocker

Software-based protection mechanisms used during acquisition.

---

# Hash Verification

Hash values are used to prove that evidence has not been altered.

Common algorithms:

- MD5
- SHA-1
- SHA-256

Matching hashes confirm integrity.

---

# Common Forensic Image Formats

## RAW / DD

- Bit-by-bit copy format
- No additional metadata
- Supported by many forensic tools

---

## E01 (Expert Witness Format)

Developed by Guidance Software.

Features:
- Compression support
- Metadata storage
- Hash information
- Evidence notes

Supported by:
- EnCase
- FTK
- Autopsy
- Magnet AXIOM

---

## AFF (Advanced Forensic Format)

Open forensic image format.

Features:
- Open standard
- Metadata support
- Compression

---

## AD1

Created by AccessData.

Used for:
- Logical acquisitions
- File and folder collections

---

# Common Imaging Tools

## FTK Imager

Used for:
- Creating forensic images
- Hash verification
- Evidence preview

## OpenText TD2U

Used for:
- Disk imaging
- Disk cloning
- Evidence acquisition

## Falcon Neo

Used for:
- High-speed forensic acquisition
- Multiple device imaging

---

# Conclusion

Proper forensic imaging ensures evidence preservation, integrity verification, and repeatable analysis during digital investigations.
