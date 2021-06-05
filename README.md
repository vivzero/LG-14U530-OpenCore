# LG 14U530 Hackintosh
It tested with macOS Catalina, and Big Sur.

## Before You Install...
1. Choose OpenShell.efi in OpenCore Boot Menu.
2. Type `FS0:`, and `ls`. 
- 2-1. If shown EFI Folder, Go to the 3.
- 2-2. If not, Type `FS1:`, and `ls`. If not too, Type `FS2`, and `ls`, ...
3. Type `cd EFI\OC\Tools`.
4. Type `ControlMsrE2.efi unlock`. Follow the instructions.
5. Press Ctrl+Alt+Del, and start installation.

## System Spec
| Components | Details |
| - | - |
| CPU | Intel Core i5-4200U |
| iGPU | Intel HD Graphics 4400 |
| dGPU | NVIDIA GeForce GT 720M |
| RAM | 2x HMT451S6BFR8A-PB |
| LCD | LP140WF1-SPJ1 (LGD0406) |
| WLAN | ~~AC 7260~~ AW-CE123H |
| Audio | Realtek ALC282 |
| BIOS | 14U530F9 (04/17/2014) |

## BIOS Setup Configs
- Legacy OS Boot: Off
- PXE Boot: Off
- xHCI Mode: Enabled
- Secure Boot Option: Off

## Reported Issues
- VGA Output works, but it has several problems related to lid and sleeping.
- Some features won't work: dGPU, SD Card Reader, Windows-only Function Keys, and hibernate mode 25.
- [Itlwm] After waking from sleep, Wi-Fi doesn't work.
- [Itlwm] Bluetooth has short range because of Wi-Fi.
- Trackpad works, but it's not good because of hardware limitation. I recommend to use Magic Trackpad 2...
- If you attempt to hibernate, mini PCIe and "Battery Charge Stop Percentage" Config (in BIOS Setup) will be lost.
