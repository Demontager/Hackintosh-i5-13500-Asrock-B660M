# Hackintosh-i5-13500-Asrock-B660M
## Hardware

| **Component**        | **Model**                                                                              |
| -------------------- | -------------------------------------------------------------------------------------- |
| CPU                  | Intel Core i5 13500                                                                   |
| Motherboard          | [Asrock B660M-ITX/ac](https://www.asrock.com/mb/Intel/B660M-ITXac/index.asp)           |
| RAM                  | 64GB (2 x 32GB) Kingston Fury Beast KF432C16BBK2/64                                                     |
| GPU                  | AMD Radeon RX 6800 - 16GB ([https://www.powercolor.com/product?id=1630396326](https://www.amd.com/en/products/graphics/amd-radeon-rx-6800) |
| OS Disk (Nvme) |  samsung 970 evo plus 2tb                                                                       |
| WiFi / Bluetooth     | Apple plug-n-play BCM94360CS2                                                  |
| Display              | 2K (Samsung) @ 144Hz                                                     |

![Screenshot 2023-06-30 at 20 37 02](https://github.com/Demontager/Hackintosh-i5-13500-Asrock-B660M/assets/7040503/232ee1cd-b092-4bab-abc6-3176ce16046c)

## BIOS Settings

### OC Tweaker

- Intel Turbo Boost Max Technology 3.0: **Enabled**

### Advanced - CPU Configuration

- Intel Hyper-Threading Technology: **Enabled**
- **CFG Lock**: **Disabled**
- Intel Virtualization Technology: **Enabled**
- **Software Guard Extensions (SGX)**: **Disabled**

### Advanced - Chipset Configuration

- Primary Graphics Adapter: **PCIe**
- Above 4G Decoding: **Enabled**
- **C.A.M (Clever Access Memory)**: **Disabled**

### Advanced - Storage Configuration

- SATA Mode Selection: **AHCI**

### Advanced - USB Configuration

- Legacy USB Support: **Enabled**
- XHCI Hand-off: **Enabled**

### Advanced - ACPI Configuration

- PS/2 Keyboard S4/S5 Wakup Support: **Enabled**
- USB Keyboard/Remote Power On: **Enabled**
- USB Mouse Power On: **Enabled**

### Advanced - Trusted Computing

- Security Device Support: **Disabled**

### Security

- **Secure Boot**: **Disabled**

### Boot

- Fast Boot: **Disabled**
- **CSM**: **Enabled**

## Tools used:
- [Opencore](https://dortania.github.io/OpenCore-Install-Guide/) 
- [ProperTree](https://github.com/corpnewt/ProperTree)
- [OpenCore Configurator](https://mackie100projects.altervista.org/download-opencore-configurator/)
- [Hackintool](https://github.com/headkaze/Hackintool)
- [SSDTTime](https://github.com/corpnewt/SSDTTime)
- [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
- [USBMap](https://github.com/corpnewt/USBMap)

## Reference

- [Dortania's OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)
- [OpenCore Alder Lake (12th-Gen Intel) Hackintosh Guidance](https://www.reddit.com/r/hackintosh/comments/sp1zgv/opencore_alder_lake_12thgen_intel_hackintosh/)
- [Fix shutdown and restart](https://github.com/Koala166/The-TLDR-Guide-of-Fixing-Shutdown-Restart)

## TO RUN DUAL MAC and WIN boot, these Quirks should be tweated as:

- DevirtualiseMmio - False
- SyncRuntimePermissions - True
