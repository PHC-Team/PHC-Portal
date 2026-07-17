# Hypervisor Guide

> **Work in Progress**
> This guide is still being updated. Information may change as new Hypervisor methods and Windows updates are released.

This guide is based partly on an article written by **RessourectoR** on **cs.rin.ru**:

https://cs.rin.ru/forum/viewtopic.php?f=10&t=156407

For readers interested in the deeper technical details behind Hypervisor bypasses and Windows security, the original article is highly recommended.

---

# What Is a Hypervisor Bypass?

Some modern Denuvo bypasses use a custom **Hypervisor** instead of modifying the game files directly.

A Hypervisor operates underneath Windows and can intercept certain CPU instructions. This allows the bypass to avoid many of Denuvo's integrity checks and anti-tamper protections without making direct changes to the game's executable.

Because Hypervisor drivers operate at a very low system level, Windows security features normally prevent them from loading. To use a Hypervisor-based bypass, some Windows security protections may need to be temporarily disabled.

After you are finished using the bypass, it is recommended to restore these security settings.

---

# Is It Safe?

Disabling Windows security features lowers some of your system's protection while they are disabled.

Possible risks include:

* Reduced protection against advanced malware
* Lower kernel-level security
* Increased risk when running untrusted software

For most users, the biggest security risk comes from downloading and running files from unreliable sources rather than from the Hypervisor itself.

Using a Hypervisor bypass is a personal choice, and you should consider the possible risks before making changes to your system.

---

# How Hypervisor Bypasses Work

Most Hypervisor-based releases consist of two main parts:

---

## 1. VBS.cmd (Windows Setup Script)

The **VBS.cmd** script prepares Windows so that Hypervisor drivers can load correctly.

It may perform tasks such as:

* Detecting incompatible Windows security features
* Disabling VBS (Virtualization-Based Security)
* Disabling Memory Integrity (Core Isolation)
* Adjusting boot configuration settings
* Restoring previous settings through the **Revert** option

This script is shared between many Hypervisor releases and is maintained separately from individual game bypasses.

---

## 2. Game-Specific Bypass Files

The second part is the actual bypass for a specific game.

It usually contains:

* Hypervisor driver
* Loader
* Game-specific DLL files
* Goldberg Steam Emulator (if required)

These files are created for specific games and versions. A bypass made for one game version will usually not work with another version.

---

# Requirements

Before using a Hypervisor-based bypass, make sure your system meets the following requirements:

* Windows 10 or Windows 11
* A CPU with virtualization support:

  * **Intel:** VT-x
  * **AMD:** AMD-V (SVM)
* CPU virtualization enabled in BIOS/UEFI

If you are unsure whether your processor supports virtualization, search for your CPU model and check its specifications.

---

# Secure Boot

## Do I Need to Disable Secure Boot?

**No.**

Modern Hypervisor bypasses do **not** require Secure Boot to be disabled and do not require EfiGuard.

---

# Frequently Asked Questions

## Do I Need to Permanently Disable Windows Security Features?

No.

The changes are intended to be temporary while using the bypass. Most setup scripts include a **Revert** option that restores your original Windows security settings afterward.

---

## Can I Use the Same Hypervisor Files for Every Game?

No.

Only the **VBS.cmd** setup script is generally shared.

The actual Hypervisor bypass files are created specifically for individual games and game versions.

---

## Why Does VBS.cmd Receive Frequent Updates?

The script is updated regularly to improve compatibility with:

* New Windows versions
* Windows security updates
* Driver loading changes
* BitLocker compatibility
* Windows Hello compatibility
* Hyper-V changes
* General bug fixes and improvements

Unless you are troubleshooting a specific issue, it is recommended to always use the latest available version.

---

# Additional Resources

For a more detailed technical explanation of Hypervisor bypasses and Windows security, see RessourectoR's original guide:

https://cs.rin.ru/forum/viewtopic.php?f=10&t=156407

---

# Request a Hypervisor Bypass

If you'd like to request a Hypervisor bypass for a Denuvo-protected game, please submit your request in our Discord server.

Before requesting a bypass, please note the following:

* Not all Denuvo-protected games currently have a Hypervisor bypass available.
* Only games listed as supported are eligible for a Hypervisor bypass.
* Check the **Supported Games** list before requesting any files.
* If a Hypervisor bypass isn't available for your game, check whether a standard Denuvo bypass is supported instead.

Thank you for your patience and understanding as we continue expanding support.