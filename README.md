# LG 14U530 Hackintosh

## Before You Install...
1. Choose CFGLock.efi in OpenCore Boot Menu.
2. Disable CFG-Lock through following the instructions on the screen.
3. Press Ctrl+Alt+Del, and start installation.

## System Specs
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
- After waking from sleep, Wi-Fi doesn't work.
- Bluetooth has short range because of Wi-Fi (Itlwm).
- When use Trackpad at first after booting, its pointing speed is faster than usual.
- Some features won't work: dGPU, SD Card Reader, Windows-only Function Keys, and hibernate mode 25.
