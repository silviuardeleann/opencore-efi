# Dell Latitude 7490 - OpenCore EFI

This folder contains a working OpenCore EFI configuration for the Dell Latitude 7490.

## 🧩 Hardware

This EFI is specifically configured for the following hardware:

- **Model:** Dell Latitude 7490
- **CPU:** Intel Core i5 / i7 8th Gen (Kaby Lake)
- **RAM:** 16GB DDR4 @ 2133 MHz (8GB/32GB Supported)
- **iGPU:** Intel UHD Graphics 620
- **SSD:** Samsung PM961 256GB M.2 NVMe
- **Ethernet:** Intel I219-V
- **Wi-Fi / Bluetooth:**  
  - Intel Wireless AC 8265 / 8260 (Requires [OpenCore Legacy Patcher](https://github.com/dortania/Opencore-Legacy-Patcher) after install to work)
  - Other cards may work with the same patches as the Intel ones.
- **Display:** 14" FHD (1920×1080)
- **Trackpad:** Precision touchpad (I2C)
- **Audio:** Realtek ALC256

## ⚙️ Features Status

### ✅ Working
- Ethernet
- WiFi / Bluetooth
- Battery status
- Sleep / Wake
- Keyboard & Trackpad
- Audio (Internal speakers and microphone)
- SD Card Reader
- USB ports (including USB-C)

### ⚠️ Partially Working
- 3.5mm Combo Jack (Works for a short period of time and glitches but eventually comes back. Also [ComboJack](https://github.com/macos86/ComboJack) needs to be installed for partial support to work / otherwise doesn't work at all.)

### ❌ Not Working
- Thunderbolt
- Smart Card Reader
- Fingerprint Reader
- WWAN/GPS (Sim slot)

## 🧰 Notes

- Make sure your BIOS settings match [OpenCore requirements](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html#intel-bios-settings) (AHCI, disabled Secure Boot unless using keys, etc.)

## 📌 Credits

OpenCore: https://github.com/acidanthera/OpenCorePkg