# Machinist X99-G7 macOS EFI

## This fork will be corrected in some days. Now it is not ready!!!

## PC configuration
| Compunent | Name |
| - | - |
| Motherboard | Machinist X99-G7 |
| CPU | Intel Xeon E5-2666v3 |
| RAM | Micron DDR3 1333MHz *(OC to 2000MHz)* |
| GPU | Saphire RX580 8Gb Pulse | 
| Storage (NVMe) | WD SN550 |
| Storage (SATA M2) 256Gb | SATA SSD 128Gb |
| Wi-Fi + BT | Broadcom BCM923602CS |

## Bugs
* Very light sleep depth (Motherboard problem)
* Built-in sound with VoodooHDA only

## Working
* CPU
* GPU
* iServices
* Wi-Fi
* Bluetooth
* NVMe
* SATA disks
* All USB ports
* Sleep (only S1)

## Installation
* Follow BIOS settings from [Dortania's guiide](https://dortania.github.io/OpenCore-Install-Guide/config-HEDT/haswell-e.html#intel-bios-settings) + XHCI mode -> Smart Auto
* **Set your own SMBIOS serial numbers in config.plist**

VoodooHDA.kext from addons have to copied to /Library/Extensions folder with command:
sudo cp -R /Path to/VoodooHDA.kext /Library/Extensions/ ; sudo chown -R root:wheel /Library/Extensions/VoodooHDA.kext ; sudo chmod -R 755  /Library/Extensions/VoodooHDA.kext 

To improove CPU performance use PMDrvr.kext driver from addons, set it up with WakeUpSCr applet. 
