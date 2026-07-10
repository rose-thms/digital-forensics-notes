# Android Forensics

## Overview

Android forensics is the process of acquiring, preserving, and analyzing digital evidence from Android devices.

Android devices contain valuable forensic artifacts such as:

- User data
- Application information
- Communication records
- Location data
- System information
- Device activity history

---

# Android Architecture

Android is built on multiple layers:
Applications
|
Application Framework
|
Android Runtime (ART)
|
Native Libraries
|
Linux Kernel

---

# Android File System

Important Android partitions:

## Boot Partition

Contains:

- Kernel
- Ramdisk
- Boot configuration


## System Partition

Contains:

- Android operating system files
- System applications


## Data Partition

Most important forensic partition.

Contains:

- User applications
- Application databases
- User settings
- Messages
- Accounts


## Cache Partition

Stores temporary system data.

---

# Android Security Model

Modern Android devices use multiple security mechanisms:

## Application Sandboxing

Each application runs in an isolated environment.

Benefits:

- Prevents unauthorized access
- Protects application data


## Permissions

Applications require permissions to access:

- Contacts
- Location
- Storage
- Camera
- Microphone

---

# Android Encryption

## Full Disk Encryption (FDE)

Used in older Android versions.

Features:

- Entire storage encrypted
- Uses device encryption keys


## File Based Encryption (FBE)

Used in modern Android versions.

Features:

- Files encrypted individually
- Supports different user profiles
- Improved security

---

# BFU and AFU States

## BFU (Before First Unlock)

Device state before the first user unlock after boot.

Limitations:

- Most user data remains encrypted
- Limited acquisition capability


## AFU (After First Unlock)

Device state after the user unlocks the device.

Advantages:

- More accessible data
- Better extraction possibilities

---

# Android Debug Bridge (ADB)

ADB is a command-line interface used to communicate with Android devices.

Common uses:

- Device information collection
- File transfer
- Debugging
- Application interaction

Example:
adb devices: Displays connected Android devices.

---

# Android Forensic Artifacts

## Call Logs

Contains:

- Incoming calls
- Outgoing calls
- Missed calls
- Timestamps


## SMS Database

Usually stored in: mmssms.db

Contains:

- Messages
- Sender information
- Timestamps


## Application Data

Applications may store:

- Messages
- User accounts
- Media
- Configuration files

Examples:

- WhatsApp databases
- Browser history
- Social media artifacts


## Location Data

Possible sources:

- GPS records
- Application location history
- Google location artifacts

---

# Android Acquisition Methods

Common acquisition methods:

## Logical Extraction

Collects accessible user data.

Examples:

- Contacts
- Messages
- Media


## File System Extraction

Collects accessible file system data.

Examples:

- Application data
- Configuration files


## Physical Extraction

Attempts to acquire raw storage data.

Challenges:

- Encryption
- Device security
- Modern protections

---

# Android Forensic Challenges

Investigators face challenges such as:

- Device encryption
- Strong authentication
- Secure boot
- Hardware-backed security
- Application encryption
- Device fragmentation

---

# Android Forensic Tools

Common tools:

- Cellebrite UFED
- Cellebrite Inseyets
- Magnet AXIOM
- MOBILedit
- XRY
- Autopsy

---

# Conclusion

Android forensics requires understanding the Android operating system, security mechanisms, acquisition techniques, and application artifacts to successfully recover and analyze digital evidence.
