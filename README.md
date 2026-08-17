# OpenCore EFI

This repository contains **OpenCore EFI** configurations for different devices.

![macOS](https://img.shields.io/badge/macOS-Sequoia-blue)
![Branch](https://img.shields.io/badge/branch-sequoia-green)

## 📦 Structure

Each device folder contains the EFI configuration and, when available, Secure Boot keys.

- `EFI/` → OpenCore bootloader and configuration files.
- `KEYS/` → Secure Boot keys for optional UEFI enrollment.

## 💻 Devices

- **Dell Latitude E7470** → [`OpenCore EFI`](./devices/Dell%20Latitude%20E7470/)
- **Dell Latitude 7490** → [`OpenCore EFI`](./devices/Dell%20Latitude%207490/)

## ⚠️ Disclaimer

These EFI configurations are intended as **device-specific starting points** for Hackintosh systems using OpenCore.

Hardware configurations can vary between units of the same model, so compatibility and required configuration may differ.

Refer to the README inside each device folder for hardware information and known compatibility.

## 📚 Resources

- [OpenCore](https://github.com/acidanthera/OpenCorePkg)
- [OpenCore Legacy Patcher](https://github.com/dortania/OpenCore-Legacy-Patcher/)
- [Dortania OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)
