# OpenCore EFI

This repository contains OpenCore EFI configurations for different devices.

![macOS](https://img.shields.io/badge/macOS-Sequoia-blue)
![Branch](https://img.shields.io/badge/branch-sequoia-green)


## 📦 Structure

Each device folder typically contains:

- `EFI/` → Main OpenCore bootloader files.
- `KEYS/` → Secure Boot keys (can be enrolled in UEFI).


## ⚠️ Notes

- These EFI folders are intended for Hackintosh setups using OpenCore.
- Secure Boot keys in `KEYS/` are optional and only needed if you want Secure Boot enabled.


## 🧭 How to Use

1. Select your device folder.
2. Copy the `EFI` folder to your EFI partition.
3. (Optional) Enroll keys from `KEYS/` into Secure Boot key store.
4. Boot and test.


## 📂 Devices

- Dell Latitude 7490 → [`Dell Latitude 7490/`](./devices/Dell%20Latitude%207490)