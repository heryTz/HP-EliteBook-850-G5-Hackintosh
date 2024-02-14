# HP EliteBook 850 G5 Hackintosh (macOS Ventura)

EFI configuration for HP EliteBook 850 G5 with macOS Ventura.

![Hackintosh demo](https://github.com/heryTz/HP-EliteBook-850-G5-Hackintosh/blob/main/demo.png)

## Setup

1. Creating the USB [↗️](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/).
2. Copy the ```EFI``` folder to the USB root
3. Install GenSMBIOS [↗️](https://github.com/corpnewt/GenSMBIOS).
4. Generate SMBIOS (use MacBookPro15,4 when generator ask the SystemProductName) [↗️](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#platforminfo).

‼️ Post-install: use [mountEFI ↗️](https://github.com/corpnewt/MountEFI) to boot macOS without the USB.

⚠️ You can see the installation details in the bootloader [OpenCore documentation ↗️](https://dortania.github.io/OpenCore-Install-Guide/).

## What works

- [x] Wifi
- [x] Speakers
- [x] Headphones output
- [x] Webcam
- [x] Trackpad with gestures
- [x] Battery percentage/status
- [x] Fn keys to change volume or brightness
- [ ] USB 3 Ports (To fix, the OS detect the device but cannot mount it)
- [ ] LAN/Ethernet (Not tested)
- [ ] HDMI Out

## System specification

```txt
─ CPU
  └── Intel(R) Core(TM) i7-8650U CPU @ 1.90GHz
      ├── SSE: SSE4.2
      ├── SSSE3: Supported
      ├── Cores: 4
      └── Threads: 8

─ Motherboard
  ├── Model: 83B2
  └── Vendor: HP

─ GPU
  └── UHD Graphics 620
      ├── Device ID: 0x5917
      ├── Vendor: 0x8086
      ├── ACPI Path: \_SB_.PCI0.GFX0
      └── PCI Path: PciRoot(0x0)/Pci(0x2,0x0)

─ Network
  ├── Ethernet Connection (4) I219-LM
  │   ├── Device ID: 0x15d7
  │   ├── Vendor: 0x8086
  │   ├── ACPI Path: \_SB_.PCI0.GLAN
  │   └── PCI Path: PciRoot(0x0)/Pci(0x1f,0x6)
  └── Wireless 8265 / 8275
      ├── Device ID: 0x24fd
      ├── Vendor: 0x8086
      ├── ACPI Path: \_SB_.PCI0.RP04.PXSX
      └── PCI Path: PciRoot(0x0)/Pci(0x1c,0x0)/Pci(0x0,0x0)

─ Audio
  └── Sunrise Point-LP HD Audio
      ├── Device ID: 0x9d71
      ├── Vendor: 0x8086
      ├── ACPI Path: \_SB_.PCI0.HDAS
      ├── PCI Path: PciRoot(0x0)/Pci(0x1f,0x3)
      └── Codec: CX8200

─ Storage
  ├── ADATA USB Flash Drive
  │   ├── Type: Hard Disk Drive (HDD)
  │   ├── Connector: SCSI
  │   └── Location: External
  └── ATA SanDisk SD9SN8W-
      ├── Type: Solid State Drive (SSD)
      ├── Connector: SCSI
      └── Location: Internal
```
