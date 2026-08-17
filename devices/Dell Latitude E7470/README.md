# Dell Latitude E7470 · OpenCore EFI

A clean, ready-to-use **OpenCore EFI** for the Dell Latitude E7470, with support for the most common hardware configurations.

> **Note:** This EFI is designed to be reusable across multiple Latitude E7470 units, but hardware variants may require minor changes to the EFI.

## 🧩 Hardware

| Component             | Supported                    |
| --------------------- | ---------------------------- |
| **CPU**               | Intel Core i5 / i7 · 6th Gen |
| **Graphics**          | Intel HD Graphics 520        |
| **RAM**               | DDR4 · 2133 MHz              |
| **Storage**           | M.2 SATA                     |
| **Ethernet**          | Intel                        |
| **Wi-Fi / Bluetooth** | Intel                        |
| **Display**           | 14" FHD / HD                 |
| **Trackpad**          | ?                            |
| **Audio**             | Realtek ALC3234              |

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
* USB

### 🟡 Not Tested

* 3.5mm Combo Jack

### 🔴 Not Working

* Smart Card Reader
* Fingerprint Reader
* WWAN / GPS

## 📡 Intel Wi-Fi / Bluetooth

Intel cards require [OpenCore Legacy Patcher](https://github.com/dortania/OpenCore-Legacy-Patcher).

Set:

```text
SecureBootModel = Disabled
```

Apply the required patches, then change it back to:

```text
SecureBootModel = Default
```

Other compatible wireless cards may work with the same patches.

## ⚙️ BIOS

Follow the [Dortania OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html#intel-bios-settings) for the recommended BIOS configuration.

At minimum, make sure **AHCI** is enabled and **Secure Boot** is configured appropriately.

## 🔧 Hardware Variants

The Latitude E7470 was shipped with different hardware configurations. Before using this EFI on another unit, check:

* Wi-Fi / Bluetooth card
* Audio codec
* Display
* Trackpad
* Storage
* CPU / iGPU

If the hardware differs, the corresponding **kexts, ACPI files, or `config.plist` settings** may need to be adjusted.

## 🙏 Credits

[Dortania](https://dortania.github.io/OpenCore-Install-Guide/) · [OpenCore](https://github.com/acidanthera/OpenCorePkg) · [OpenCore Legacy Patcher](https://github.com/dortania/OpenCore-Legacy-Patcher)
