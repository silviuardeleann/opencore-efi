# Dell Latitude 7490 · OpenCore EFI

A clean, ready-to-use **OpenCore EFI** for the Dell Latitude 7490, with support for the most common hardware configurations.

> **Note:** This EFI is designed to be reusable across multiple Latitude 7490 units, but hardware variants may require minor changes to the EFI.

## 🧩 Hardware

| Component             | Supported                    |
| --------------------- | ---------------------------- |
| **CPU**               | Intel Core i5 / i7 · 8th Gen |
| **Graphics**          | Intel UHD Graphics 620       |
| **RAM**               | DDR4 · 2133 MHz              |
| **Storage**           | M.2 NVMe                     |
| **Ethernet**          | Intel I219-V                 |
| **Wi-Fi / Bluetooth** | Intel 8260 / 8265            |
| **Display**           | 14" FHD · 1920×1080          |
| **Trackpad**          | I2C Precision Touchpad       |
| **Audio**             | Realtek ALC256               |

## ✨ Compatibility

### 🟢 Working

* Ethernet
* Wi-Fi & Bluetooth*
* Battery & power management
* Sleep / Wake
* Keyboard & Trackpad
* Internal Audio & Microphone
* Webcam
* SD Card Reader
* USB & USB-C

### 🟡 Partial

* **3.5mm Combo Jack** — intermittent; requires [ComboJack](https://github.com/macos86/ComboJack)

### 🔴 Not Working

* Thunderbolt
* Smart Card Reader
* Fingerprint Reader
* WWAN / GPS

## 📡 Intel Wi-Fi / Bluetooth

Intel **8260 / 8265** cards require [OpenCore Legacy Patcher](https://github.com/dortania/OpenCore-Legacy-Patcher).

Set:

```text
SecureBootModel = Disabled
```

Apply the required patches, then change it back to:

```text
SecureBootModel = j132
```

Other compatible wireless cards may work with the same patches.

## ⚙️ BIOS

Follow the [Dortania OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html#intel-bios-settings) for the recommended BIOS configuration.

At minimum, make sure **AHCI** is enabled and **Secure Boot** is configured appropriately.

## 🔧 Hardware Variants

The Latitude 7490 was shipped with different hardware configurations. Before using this EFI on another unit, check:

* Wi-Fi / Bluetooth card
* Audio codec
* Display
* Trackpad
* Storage
* CPU / iGPU

If the hardware differs, the corresponding **kexts, ACPI files, or `config.plist` settings** may need to be adjusted.

## 🙏 Credits

[Dortania](https://dortania.github.io/OpenCore-Install-Guide/) · [OpenCore](https://github.com/acidanthera/OpenCorePkg) · [OpenCore Legacy Patcher](https://github.com/dortania/OpenCore-Legacy-Patcher) · [ComboJack](https://github.com/macos86/ComboJack)
