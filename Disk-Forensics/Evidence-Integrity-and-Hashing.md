# Evidence Integrity and Hashing

## Overview

Maintaining evidence integrity is one of the most important principles in digital forensics.

A forensic examiner must ensure that the original evidence remains unchanged from the time of acquisition until the completion of analysis.

Hashing is used to verify that digital evidence has not been modified.

---

# Digital Evidence Integrity

Digital evidence integrity means:

- Evidence is preserved in its original state
- No unauthorized modifications occur
- Analysis can be repeated and verified
- Findings are reliable

To maintain integrity, forensic investigators use:

- Write blockers
- Hash verification
- Proper documentation
- Chain of custody

---

# Hash Functions

A hash function converts data of any size into a fixed-length value called a hash value.

Example:
Evidence File
|
↓
Hash Algorithm
|
↓
Unique Hash Value

Even a small change in data will produce a different hash value.

---

# Common Hash Algorithms

## MD5

Hash Length: 128 bits

Uses:

- Quick integrity checks
- Legacy forensic workflows

Limitations:

- Collision vulnerabilities

---

## SHA-1

Hash Length: 160 bits

Uses:

- Previously common in forensic tools

Limitations:

- Reduced security due to collision attacks

---

## SHA-256

Hash Length: 256 bits

Currently widely used for forensic verification.

Advantages:

- Strong collision resistance
- Reliable evidence validation

---

# Hash Verification Process

Typical forensic workflow:

## Step 1: Calculate Original Evidence Hash

Example: 
Original Drive Hash:

SHA-256:
8a7f9c4dxxxxxxxx

---

## Step 2: Create Forensic Image

The storage device is acquired using a forensic imaging tool.

Examples:

- FTK Imager
- OpenText TD2U
- Falcon Neo

---

## Step 3: Calculate Image Hash

Example: 
Image Hash:

SHA-256:
8a7f9c4dxxxxxxxx

---

## Step 4: Compare Hash Values

If both hashes match: Original Evidence Hash = Image Hash

The forensic image is considered verified.

---

# Hashing in Forensic Tools

## FTK Imager

Used for:

- Creating forensic images
- Calculating hash values
- Verifying acquisition

---

## Magnet AXIOM

Uses hash information during:

- Evidence processing
- File identification
- Analysis

---

## Cellebrite UFED

Uses integrity verification during:

- Mobile acquisition
- Extraction validation

---

# Chain of Custody Connection

Hash values support chain of custody by proving:

- Evidence remained unchanged
- Acquisition was successful
- Analysis was performed on a verified copy

Documentation should include:

- Evidence ID
- Date and time
- Examiner details
- Hash values
- Acquisition method

---

# Conclusion

Hash verification is a critical step in digital forensic investigations. It ensures that evidence remains authentic, reliable, and suitable for forensic examination.






