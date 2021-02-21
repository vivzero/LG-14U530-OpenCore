# LG 14U530 Hackintosh

## Before Install...
1. You should modify PlatformInfo Section in config.plist.
2. You have to choose "CFGLock.efi" in boot menu.

[MountEFI](https://github.com/corpnewt/MountEFI) is used to mount EFI Partition.
[ProperTree](https://github.com/corpnewt/ProperTree) and [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) is used to modify config.plist.

You can also refer to "OpenCore Install Guide" by Dortania.

## Specifications 
| Component | Details |
| - | - |
| CPU | Intel Core i5-4200U |
| iGPU | Intel HD Graphics 4400 |
| dGPU | Nvidia GeForce GT 720M |
| RAM | Apple HMT451S6BFR8A-PB * 2 |
| SSD | SK hynix HFS128G3AMNB-2200A |
| HDD | TOSHIBA MQ01ABD050 |
| LCD | 14-inch IPS, 1920 * 1080 |
| WLAN | Intel Dual Band AC 7260 |

## It works Partially
- Wi-Fi
- Bluetooth
- VGA Port : Unplugging detection is missing.

## It does not work
- dGPU (Optimus)
- SD Card Reader (RTS5129)
- Windows-only Function Keys
- Hibernation (Mode 25)