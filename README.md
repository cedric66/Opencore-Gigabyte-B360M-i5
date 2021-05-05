# Opencore-Gigabyte-B360M-i5

## Specs
```
Motherboard : Gigabyte B360 Aorus Gaming 3

Processor : Intel Core i5-8600 (Coffee Lake) 

Ram: Transcend 24GB DDR4 

SSD : Crucial 250GB SATA 

Graphics : Intel UHD Graphics 630 2048 MB

WIFI & Bluetooth : Asus PCE-AX3000 AX3000 Dual Band PCI-E WiFi 6 (802.11ax), Bluetooth 5.0

Ethernet : Intel I219V7 PCI Express Gigabit- Ethernet
```

## Software
- OpenCore 0.6.8
- macOS Big Sur 11.3

## What works
4K/60/10 bit DisplayPort output, analog audio, sleep/wake, Wi-Fi and Bluetooth, Continuity, FileVault, Software DRM etc.
## BIOS Setting
### Disable
```
* Fast Boot
* Secure Boot
* Serial/COM Port
* VT-d
* Intel Platform Trust

```
### Enable
```
* Above 4G decoding
* Hyper-Threading
* EHCI/XHCI Hand-off
* DVMT Pre-Allocated(iGPU Memory): 64MB
* SATA Mode: AHCI
```
## Change Serial,MLB,SMUUID

At first download GenSMBIOS tool from [here.](https://github.com/corpnewt/GenSMBIOS)

Then extract it & Open-> GenSMBIOS.command

#### 1. Select option :3

#### 2. type: iMac19,2

#### 3. Copy the Serial, Board Serial & SmUUID

#### 4. Open EFI->OC->config.plist then Replace it with your generated SMBIOS
```
Serial -> SystemSerialNumber
Board Serila -> MLB
SmUUID ->SystemUUID
```

## Guide<br>
* [Open Core Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)
## Credit<br>
* - Thanks to [sohagmahin](https://github.com/sohagmahin), [Acidanthera](https://github.com/acidanthera) for providing [AppleALC](https://github.com/acidanthera/AppleALC), [HibernationFixup](https://github.com/acidanthera/HibernationFixup), [Lilu](https://github.com/acidanthera/Lilu), [NVMeFix](https://github.com/acidanthera/NVMeFix), [OcBinaryData](https://github.com/acidanthera/OcBinaryData), [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg), [RestrictEvents](https://github.com/acidanthera/RestrictEvents), [VirtualSMC](https://github.com/acidanthera/VirtualSMC), [VoodooInput](https://github.com/acidanthera/VoodooInput), [VoodooPS2](https://github.com/acidanthera/VoodooPS2), and [WhateverGreen](https://github.com/acidanthera/WhateverGreen).
