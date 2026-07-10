# iOS Forensics

## Overview

iOS forensics is the process of acquiring, preserving, and analyzing digital evidence from Apple devices such as iPhones and iPads.

iOS devices contain valuable forensic artifacts including:

- Messages
- Call history
- Application data
- Photos and videos
- Location information
- Browser activity
- Device metadata

---

# iOS Architecture

The iOS ecosystem consists of multiple security layers:
Applications
|
Cocoa Touch Framework
|
Core Services
|
Core OS
|
Hardware

Each layer contributes to device functionality and security.

---

# iOS Security Model

Apple uses multiple security mechanisms to protect user data.

## Secure Boot Chain

Ensures that only trusted software is loaded during device startup.

Process:
Boot ROM
↓
Low Level Bootloader (LLB)
↓
iBoot
↓
iOS Kernel

---

## Secure Enclave

The Secure Enclave is a dedicated hardware security component.

Responsibilities:

- Protect encryption keys
- Manage biometric authentication
- Protect sensitive operations

Used with:

- Touch ID
- Face ID
- Device encryption

---

# iOS Encryption

Modern iOS devices use hardware-backed encryption.

Important concepts:

## Data Protection Classes

iOS protects files based on accessibility levels.

Examples:

- Complete Protection
- Protected Until First User Authentication
- Protected Unless Open

---

# BFU and AFU States

## BFU (Before First Unlock)

State before the device is unlocked after reboot.

Characteristics:

- Encryption keys are unavailable
- Limited data access
- Strong protection enabled


## AFU (After First Unlock)

State after the user unlocks the device.

Characteristics:

- More keys available
- Greater data accessibility
- More artifacts can be acquired

---

# iOS Acquisition Methods

## Logical Extraction

Collects accessible user data.

Examples:

- Contacts
- Messages
- Media
- Device information


## Advanced Logical Extraction

May collect additional application artifacts depending on device and security state.


## File System Extraction

Provides access to a larger amount of iOS file system data.

Can include:

- Application containers
- Databases
- Configuration files


## Full File System Extraction

Attempts to acquire the complete accessible file system.

Availability depends on:

- Device model
- iOS version
- Security protections

---

# iOS Forensic Artifacts

## Messages

Contains:

- iMessage data
- SMS messages
- Attachments
- Timestamps


## Call History

Contains:

- Incoming calls
- Outgoing calls
- Missed calls
- Contact information


## Application Data

Applications may contain:

- User accounts
- Chat databases
- Media
- Configuration information


## Photos and Media

Artifacts include:

- Images
- Videos
- EXIF metadata
- Creation timestamps
- Location information

---

# iOS Backup Analysis

iOS backups can contain valuable forensic evidence.

Types:

## Encrypted Backup

Provides stronger protection.

Requires:

- Backup password
- Proper authentication


## Unencrypted Backup

Contains accessible user data but provides less protection.

---

# Keychain

The iOS Keychain stores sensitive information:

- Passwords
- Authentication tokens
- Encryption keys
- Certificates

Access depends on device security state.

---

# iOS Forensic Tools

Common tools:

- Cellebrite UFED
- Cellebrite Inseyets
- Magnet AXIOM
- MOBILedit
- XRY

---

# Challenges in iOS Forensics

Investigators face challenges such as:

- Strong encryption
- Secure Enclave protections
- Passcode protection
- Limited access after reboot
- iOS version changes

---

# Conclusion

iOS forensics requires understanding Apple's security architecture, encryption mechanisms, acquisition methods, and artifact locations to properly analyze digital evidence.
