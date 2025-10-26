# URumble – Universal Rumble & Haptics Enabler

**Version 1.0 – By TonyStyle**

---

## Description

URumble is **not magic**. This module does **not install new drivers**, does **not patch your kernel**, and does **not create features that aren’t already present** on your device.  

What it does:  

- **Enables Force Feedback, Rumble, and Haptics** that are already in your kernel or ROM but were disabled by the manufacturer.  
- Loads available HID and uinput modules to maximize compatibility with **all controllers** (DualSense, DualShock, Xbox, Nintendo, Logitech, etc.).  
- Automatically reapplies sysfs flags and system properties to keep rumble / haptics active after boot.  

In short: **if your device or controller supports feedback, this module unlocks it. Otherwise, it can’t create something that doesn’t exist.**  

---

## Installation

1. Download the ZIP file.  
2. Flash via Magisk Manager.  
3. Reboot.  
4. Connect a controller and test rumble / haptics.  

---

## Debug


Check `/dev/uinput` and `/sys/class/input/*/device/ff_effects` exist.

---

## Disclaimer

**This module is provided “as-is”.** I am **not responsible** if the module does not work on your device, if your controller is unsupported, or if any side effects occur. Use at your own risk.
