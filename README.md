# Machinist X99-G7 macOS EFI

## Use only zip folder X99G7-2666v3-RX580!!!

## PC configuration
| Component | Name |
| - | - |
| Motherboard | Machinist X99-G7 |
| CPU | Intel Xeon E5-2666v3 |
| RAM | Desktop DDR3 1867 MHz |
| GPU | Sapphire RX580 8Gb Pulse | 
| Storage (NVMe) | WD SN550 |
| Storage (SATA) | M2 256Gb + SATA SSD 128Gb |
| Wi-Fi + BT | Broadcom BCM923602CS |

## Bugs
* Very light sleep depth (Motherboard problem)

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
* FileVault2
  

## Installation
* Stock BIOS fix memory 1867 MHz
* XHCI mode -> Smart Auto
* **Set your own SMBIOS serial numbers in config.plist**

If you want VoodooHDA.kext instead of AppleAlc, the kext from addons have to be copied to /Library/Extensions folder with command:
sudo cp -R /Path to/VoodooHDA.kext /Library/Extensions/ ; sudo chown -R root:wheel /Library/Extensions/VoodooHDA.kext ; sudo chmod -R 755  /Library/Extensions/VoodooHDA.kext
Confirm in the system settings load the extensions.
Disable AppleAlc kext and enable AppleHDADisabler.kext in OpenCore config.plist


To improve CPU performance use PMDrvr.kext driver from addons, set it up with WakeUpSCr applet.
Confirm in the system settings
