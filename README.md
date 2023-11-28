# Machinist X99-G7 macOS EFI

## PC configuration
| Compunent | Name |
| - | - |
| Motherboard | Machinist X99-G7 |
| CPU | Intel Xeon E5-2666v3 |
| RAM | Micron DDR3 1333MHz *(OC to 2000MHz)* |
| GPU | Saphire RX580 Trixx 8Gb | 
| Storage (NVMe) | Samsung EVO 980 1TB |
| Storage (SATA) | Apacer AS350 256GB *(macOS disk)*, WD Red 2TB |
| Wi-Fi + BT | Broadcom BCM923602CS |

## Requirements
* Custom BIOS for some hidden settings
* ACPI Sleep State -> S1 **(S3 doesn't work at all on this motherboard!)**

## Bugs
* Shutdown (PC reboots instead of shutdown)
* Very light sleep depth (Motherboard problem)
* Updates are installing from the second time only (macOS downloads full installer after one unsuccessful update attempt)
* DVI port not working - VBIOS problem

## Not tested
* AirPort, AirDrop
* HDMI
* Front panel USB3 port in USB3 mode
* Audio jacks (I am Bluetooth enjoyer :b)

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
* You should know other steps yourself cuz I'm too lazy to write them here
