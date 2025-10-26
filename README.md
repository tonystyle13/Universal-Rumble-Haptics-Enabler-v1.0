# 🌀 Universal Rumble & Haptics Enabler

**By TonyStyle**

This Magisk module attempts to unlock and enable all available **rumble, vibration, and haptic feedback features** that already exist in your Android kernel and drivers — especially for **Bluetooth and USB gamepads** (PlayStation, Xbox, generic HID, etc.).

It doesn’t add new drivers or modify your system libraries — it only **forces activation** of features that manufacturers often leave disabled by default.

---

## ⚡ What It Does

* Loads common **force feedback and HID modules** (`hid_playstation`, `hid_xpad`, `hid_sony`, `uinput`, `ff-memless`, etc.)
* Enables **system-wide haptic flags** (`persist.sys.ff.enable`, `persist.sys.haptics.enable`, etc.)
* Applies **maximum permissions** on input and vibration devices for compatibility
* Forces **FF (Force Feedback)** activation in kernel parameters
* Keeps `uinput` ready for real-time rumble injection
* Auto-refreshes every minute to ensure persistent activation

---

## 🧠 Important Notes

> **This module does NOT perform magic.**
> It only enables what your device already supports.
> If your kernel or Bluetooth stack doesn’t implement rumble, it won’t suddenly start vibrating — that’s not how physics (or drivers) work.

This module is meant to **help developers, modders, and tinkerers** who already have partial rumble/haptic functionality but want to ensure **maximum activation and compatibility** across devices.

---

## ⚙️ Compatibility

* Works on **Android 10–14+**
* Requires **Magisk v24 or higher**
* Compatible with **both ARM64 and x86_64** devices
* Tested on:

  * Lenovo Pad M9 (MTK)
  * Xiaomi Pad 5 (Snapdragon)
  * Various Bluetooth gamepads (DS4, DS5, Xbox, 8BitDo, etc.)

---

## 📦 Installation

1. Download the latest release from [Releases](../../releases).
2. Flash it in **Magisk Manager → Modules → Install from storage**.
3. Reboot your device.
4. Connect your controller and test vibration (e.g. via “Gamepad Tester” app).

---

## 🧾 Changelog (summary)

**v1.0 – Initial Release**

* Added post-fs-data and service scripts
* Universal HID/FF module loading
* Force feedback enable loop
* Full permission and uinput activation
* System properties for haptic flags

---

## ⚠️ Disclaimer

This module:

* Does **not** modify any system files permanently
* Does **not** include copyrighted binaries or drivers
* Is provided **as-is**, without warranty or guarantee of function
* May not work on all devices — your mileage may vary

> **If it doesn’t work, it means your device doesn’t support it.**
> Don’t open issues complaining about “no vibration” unless you’ve confirmed your kernel includes FF/HID support.

---

## 💬 Credits

* Created by **TonyStyle**
* Special thanks to the Magisk and Android modding community
* Inspired by kernel devs who left cool features locked behind flags

---

## 📜 License

This project is released under the **MIT License** — you can modify, redistribute, and use it freely as long as credit is preserved.

---

> *Because rumble should never be optional.*
