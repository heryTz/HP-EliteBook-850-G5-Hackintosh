# HP EliteBook 850 G5 Hackintosh (macOS Ventura)

EFI configuration for HP EliteBook 850 G5 with macOS Ventura.

## Setup

1. Creating the USB [↗️](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/).
2. Copy the ```EFI``` folder to the USB root
3. Install GenSMBIOS [↗️](https://github.com/corpnewt/GenSMBIOS).
4. Generate SMBIOS (use MacBookPro15,4 when generator ask the SystemProductName) [↗️](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#platforminfo).

‼️ Post-install: use [mountEFI ↗️](https://github.com/corpnewt/MountEFI) to boot macOS without the USB.

⚠️ You can see the installation details in the bootloader [OpenCore documentation ↗️](https://dortania.github.io/OpenCore-Install-Guide/).

## What works

[x] Wifi

[x] Speakers

[x] Headphones output

[x] Webcam

[x] Trackpad with gestures

[x] Battery percentage/status

[x] Fn keys to change volume or brightness

[ ] USB 3 Ports (To fix, the OS detect the device but cannot mount it)

[ ] LAN/Ethernet (Not tested)

[ ] HDMI Out
