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
| WLAN | Intel Dual Band AC 7260 |
| Audio | Realtek ALC282 |
| BIOS | 14U530F9 (04/17/2014) |

## BIOS Setup Configs
- Legacy OS Boot: Off
- PXE Boot: Off
- xHCI Mode: Enabled
- Secure Boot Option: Off

## Reported Issues
- VGA Output works, but disconnect detection is not working.
- Some features won't work: dGPU, SD Card Reader, Windows-only Function Keys, and hibernate mode 25.
- After waking from sleep, Wi-Fi doesn't work.
- [Itlwm] Bluetooth has short range because of Wi-Fi.
- [VoodooPS2] When using Trackpad at first after booting, its pointing is odd.
- If you attempt to hibernate, mini PCIe (Intel WLAN) and "Battery Charge Stop Percentage" Config will be lost.
