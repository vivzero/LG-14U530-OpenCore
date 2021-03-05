# LG 14U530 Hackintosh

## Before Install...
- You have to choose "CFGLock.efi" in boot menu.

## Specification
| Component | Details |
| - | - |
| CPU | Intel Core i5-4200U |
| iGPU | Intel HD Graphics 4400 |
| dGPU | Nvidia GeForce GT 720M |
| RAM | Apple HMT451S6BFR8A-PB * 2 |
| LCD | LP140WF1-SPJ1 (LGD0406) |
| WLAN | Intel Dual Band AC 7260 |
| Audio | Realtek ALC282 (Layout ID: 86) |
| BIOS (UEFI) | 14U530F9 (04/17/2014) |

## BIOS Settings
- Legacy OS Boot: Off
- PXE Boot: Off
- xHCI Mode: Enabled (In BIOS Settings)
- Secure Boot Option: Off

## Reported Issues
1. Intel Wi-Fi & Bluetooth are unstable.
- Wi-Fi doesn't work after waking up from sleep.
- Bluetooth has short range because of AirportItlwm.
2. VGA works, but unplugging detection is broken.
3. Touchpad pointing speed is slightly faster after boot.
4. Booting is slower than Windows.
5. Some features don't work.
- dGPU (GT720M)
- SD Card Reader (RTS5129)
- Windows-only Function Keys
- Hibernation (Mode 25)
