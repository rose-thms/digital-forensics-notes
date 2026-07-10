# Windows Forensic Artifacts

## Overview

Windows forensic artifacts are traces created by the operating system, applications, and user activities. These artifacts help investigators reconstruct events and identify user behavior.

Common Windows artifacts include:

- Registry
- Event Logs
- Prefetch Files
- Browser History
- USB Device History
- File System Metadata

---

# Windows Registry

## Overview

The Windows Registry is a hierarchical database that stores configuration information about:

- Operating system settings
- User preferences
- Installed applications
- Hardware information
- User activity

Important Registry Hives:

| Hive | Purpose |
|---|---|
| SAM | Local user account information |
| SYSTEM | System configuration |
| SOFTWARE | Installed software information |
| NTUSER.DAT | User-specific settings |
| SECURITY | Security-related information |

---

# Event Logs

Windows Event Logs record system and security activities.

Location:
C:\Windows\System32\winevt\Logs


Important Logs:

## Security Log

Used for:

- Login attempts
- Account changes
- Privilege usage

Examples:
Event ID 4624 - Successful Logon

Event ID 4625 - Failed Logon

---

## System Log

Contains:

- System startup/shutdown
- Driver activities
- Hardware events

---

## Application Log

Contains:

- Application errors
- Program events

---

# Prefetch Files

Location:
C:\Windows\Prefetch


Purpose:

Windows Prefetch records application execution activity.

Can reveal:

- Executed programs
- Execution frequency
- Last execution time

Example: CHROME.EXE-XXXX.pf


---

# USB Device History

USB artifacts help identify external devices connected to a system.

Important locations:

Registry: HKLM\SYSTEM\CurrentControlSet\Enum\USBSTOR


Information available:

- Device manufacturer
- Serial number
- Connection history

---

# Browser Artifacts

Browsers store:

- History
- Cookies
- Downloads
- Saved credentials
- Cache

Common locations:

Chrome: User Profile\AppData\Local\Google\Chrome\User Data
Edge: User Profile\AppData\Local\Microsoft\Edge\User Data


---

# File System Metadata

Important timestamps:

## MACB Timeline

M - Modified

A - Accessed

C - Changed

B - Birth/Created


These timestamps help investigators build event timelines.

---

# Common Windows Forensic Tools

## Autopsy

Used for:
- Disk analysis
- Artifact extraction
- Timeline analysis


## FTK Imager

Used for:
- Evidence acquisition
- File preview


## Magnet AXIOM

Used for:
- Artifact processing
- Timeline creation
- Reporting


## Velociraptor

Used for:
- Endpoint artifact collection
- Incident response

---

# Conclusion

Windows artifacts provide valuable evidence for reconstructing user activity, system events, and security incidents during digital forensic investigations.




