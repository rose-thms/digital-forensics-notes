# UFED Extraction Types

## Overview

Cellebrite UFED (Universal Forensic Extraction Device) is a forensic acquisition tool used to extract digital evidence from mobile devices.

The extraction method depends on:
- Device model
- Operating system
- Security configuration
- Available access level

---

# Types of Mobile Extractions

## 1. Logical Extraction

### Description
Logical extraction collects data through standard device communication protocols without accessing the physical storage.

### Commonly Extracted Data
- Contacts
- Call logs
- Messages
- Calendar
- Media files
- Application data (limited)

### Advantages
- Fast acquisition
- Lower risk
- Supported on many devices

### Limitations
- Cannot access deleted data
- Limited artifact availability

---

## 2. Advanced Logical Extraction

### Description
An enhanced logical extraction method that retrieves additional artifacts using vendor-specific methods.

### Can Include
- Application databases
- Additional messages
- Device information
- More application artifacts

---

## 3. File System Extraction

### Description
File System extraction accesses the device file system to collect a larger amount of data compared to logical extraction.

### Common Artifacts
- Application databases
- System files
- User data
- Configuration files

### Advantages
- More detailed analysis
- Access to application-level artifacts

---

## 4. Full File System Extraction

### Description
Full File System extraction attempts to acquire the complete accessible file system of the device.

### Used For
- Advanced investigations
- Detailed artifact analysis
- Application examination

---

## 5. Physical Extraction

### Description
Physical extraction involves acquiring a bit-by-bit copy of the device storage.

### Advantages
- Potential recovery of deleted data
- Deep forensic analysis

### Challenges
- Device compatibility limitations
- Encryption protections

---

# Extraction Selection Factors

The examiner considers:

- Device model
- Android/iOS version
- Lock status
- Encryption state
- Available exploits
- Investigation requirements

---

# Note

The choice of extraction method depends on the forensic objective and the access level available on the device.
