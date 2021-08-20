# LG 14U530 Hackintosh
It tested with macOS Catalina, and Big Sur.

![](Image.jpeg)

## Before You Install...
- You should type `ControlMsrE2.efi unlock` by using OpenShell.efi.
- __Or__ enable `AppleXcpmCfgLock` in config.plist.

## System Spec
| Components | Details |
| - | - |
| CPU | Intel Core i5-4200U |
| iGPU | Intel HD Graphics 4400 |
| dGPU | NVIDIA GeForce GT 720M |
| RAM | 2x HMT451S6BFR8A-PB |
| LCD | LP140WF1-SPJ1 (LGD0406) |
| WLAN | AC 7260 |
| Audio | Realtek ALC282 |
| BIOS | 14U530F9 (04/17/2014) |

## BIOS Setup Configs
- Legacy OS Boot: Off
- PXE Boot: Off
- xHCI Mode: Enabled
- Secure Boot Option: Off

## Reported Issues
- Some features won't work: DGPU, SD Card reader, and hibernation.
- VGA Output works, but it has several problems related to lid and sleeping.
- If you attempt to hibernation, mPCIe Device (WLAN) will be disabled.
- Itlwm, for Intel WLAN, has some problems: Wi-Fi is gone after sleeping, and Bluetooth is unstable.
- (OC 0.7.2) Currently, Kernel Panic is shown sometimes when booting. I think that latest Bluetooth kext is problematic.
