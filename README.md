<div align="center">

# Intel I225 / I226 NVM Firmware

NVM firmware images for the Intel® Ethernet Controller I225-V, I226-V, I226-LM and I226-IT,<br>in 1 MB and 2 MB flash sizes.

</div>

---

Intel doesn't publish a standalone NVM update for the I226 family. It leaves firmware to board makers, and many boards still ship 2.14 or 2.17, which predate Intel's fixes for link drops and enumeration failures. This repository keeps every image in one place.

## Downloads

The latest image for each controller and flash size.

| Controller | PCI ID | 1 MB flash | 2 MB flash |
|:--|:--|:--|:--|
| **I226-V** | `8086:125C` | [**v2.36**](https://github.com/BillyCurtis/Intel-I226-V-NVM-Firmware/raw/main/I226-V/2.36/FXVL_125C_V_1MB_2.36.bin) · `80000425` | [**v2.37**](https://github.com/BillyCurtis/Intel-I226-V-NVM-Firmware/raw/main/I226-V/2.37/FXVL_125C_V_2MB_2.37.bin) · `80000422` |
| **I226-LM** | `8086:125B` | [**v2.36**](https://github.com/BillyCurtis/Intel-I226-V-NVM-Firmware/raw/main/I226-LM/2.36/FXVL_125B_LM_1MB_2.36.bin) · `80000424` | [**v2.37**](https://github.com/BillyCurtis/Intel-I226-V-NVM-Firmware/raw/main/I226-LM/2.37/FXVL_125B_LM_2MB_2.37.bin) · `80000421` |
| **I226-IT** | `8086:125D` | [**v2.32**](https://github.com/BillyCurtis/Intel-I226-V-NVM-Firmware/raw/main/I226-IT/2.32/FXVL_125D_IT_1MB_2.32.bin) · `80000433` | [**v2.32**](https://github.com/BillyCurtis/Intel-I226-V-NVM-Firmware/raw/main/I226-IT/2.32/FXVL_125D_IT_2MB_2.32.bin) · `80000431` |
| **I225-V** | `8086:15F3` | [**v1.89**](https://github.com/BillyCurtis/Intel-I226-V-NVM-Firmware/raw/main/I225-V/1.89/FXVL_15F3_V_1MB_1.89.bin) · `800002FC` | [**v1.89**](https://github.com/BillyCurtis/Intel-I226-V-NVM-Firmware/raw/main/I225-V/1.89/FXVL_15F3_V_2MB_1.89.bin) · `800002F4` |

> From 2.27 onward, the EtrackID no longer changes between versions. The update tool may report a card on 2.27 or later as up to date. Compare the **NVM version** instead, and update with `-f`.

## Version history

### I226-V

PCI ID `8086:125C`

| Version | 1 MB | 2 MB |
|:--|:--|:--|
| **2.37** | — | [`80000422`](I226-V/2.37/FXVL_125C_V_2MB_2.37.bin) |
| **2.36** | [`80000425`](I226-V/2.36/FXVL_125C_V_1MB_2.36.bin) | [`80000422`](I226-V/2.36/FXVL_125C_V_2MB_2.36.bin) |
| 2.32 | [`80000425`](I226-V/2.32/FXVL_125C_V_1MB_2.32.bin) | [`80000422`](I226-V/2.32/FXVL_125C_V_2MB_2.32.bin) |
| 2.27 | [`80000425`](I226-V/2.27/FXVL_125C_V_1MB_2.27.bin) | [`80000422`](I226-V/2.27/FXVL_125C_V_2MB_2.27.bin) |
| 2.25 | — | [`800003AD`](I226-V/2.25/FXVL_125C_V_2MB_2.25.bin) |
| 2.23 | [`8000039D`](I226-V/2.23/FXVL_125C_V_1MB_2.23.bin) | — |
| 2.22 | — | [`80000371`](I226-V/2.22/FXVL_125C_V_2MB_2.22.bin) |
| 2.17 | [`80000308`](I226-V/2.17/FXVL_125C_V_1MB_2.17.bin) | [`80000303`](I226-V/2.17/FXVL_125C_V_2MB_2.17.bin) |
| 2.14 | [`80000290`](I226-V/2.14/FXVL_125C_V_1MB_2.14.bin) | [`8000028D`](I226-V/2.14/FXVL_125C_V_2MB_2.14.bin) |
| 2.13 | — | [`80000284`](I226-V/2.13/FXVL_125C_V_2MB_2.13.bin) |

### I226-LM

PCI ID `8086:125B`

| Version | 1 MB | 2 MB |
|:--|:--|:--|
| **2.37** | — | [`80000421`](I226-LM/2.37/FXVL_125B_LM_2MB_2.37.bin) |
| **2.36** | [`80000424`](I226-LM/2.36/FXVL_125B_LM_1MB_2.36.bin) | [`80000421`](I226-LM/2.36/FXVL_125B_LM_2MB_2.36.bin) |
| 2.32 | [`80000424`](I226-LM/2.32/FXVL_125B_LM_1MB_2.32.bin) | [`80000421`](I226-LM/2.32/FXVL_125B_LM_2MB_2.32.bin) |
| 2.17 | [`80000307`](I226-LM/2.17/FXVL_125B_LM_1MB_2.17.bin) | [`80000302`](I226-LM/2.17/FXVL_125B_LM_2MB_2.17.bin) |

### I226-IT

PCI ID `8086:125D`

| Version | 1 MB | 2 MB |
|:--|:--|:--|
| **2.32** | [`80000433`](I226-IT/2.32/FXVL_125D_IT_1MB_2.32.bin) | [`80000431`](I226-IT/2.32/FXVL_125D_IT_2MB_2.32.bin) |

### I225-V

PCI ID `8086:15F3`

| Version | 1 MB | 2 MB |
|:--|:--|:--|
| **1.89** | [`800002FC`](I225-V/1.89/FXVL_15F3_V_1MB_1.89.bin) | [`800002F4`](I225-V/1.89/FXVL_15F3_V_2MB_1.89.bin) |
| 1.68 | [`800001CE`](I225-V/1.68/FXVL_15F3_V_1MB_1.68.bin) | [`800001C7`](I225-V/1.68/FXVL_15F3_V_2MB_1.68.bin) |
| 1.57 | [`80000182`](I225-V/1.57/FXVL_15F3_V_1MB_1.57.bin) | [`80000185`](I225-V/1.57/FXVL_15F3_V_2MB_1.57.bin) |
| 1.45 | [`80000150`](I225-V/1.45/FXVL_15F3_V_1MB_1.45.bin) | [`8000014B`](I225-V/1.45/FXVL_15F3_V_2MB_1.45.bin) |

## Release notes

These notes cover the onboard I226-V, I226-LM and I226-IT. Intel hasn't published notes for 2.36 or 2.37.

| Version | Changes |
|:--|:--|
| **2.37** | No public release notes. The PHY firmware build is unchanged from 2.27 (`88B6`). EFI driver `1.0.5` (2 MB), the same as 2.36. |
| **2.36** | No public release notes. The PHY firmware build is unchanged from 2.27 (`88B6`). EFI driver `1.0.5` (2 MB), a new, smaller driver that replaces `0.10.06`. |
| **2.32** | Fixes MDI lane-swap handling that could swap the P/N signal polarities incorrectly. |
| **2.27** | PHY FW `4C08_88B6`, EFI driver `0.10.06` (2 MB). Fixes the external loopback test failure seen on 2.25 (HSD 13012034657). |
| **2.25** | PHY FW `4C08_08A6`, EFI driver `0.10.06` (2 MB). Fixes link flaps with EEE enabled (HSD 13010560068). Fixes an unexpected 1 Gbps to 100 Mbps downgrade during auto-negotiation with EEE disabled (HSD 13011274310). |
| **2.23** | PHY FW `4C08_889D`, EFI driver `0.10.06` (2 MB). Fixes the device not enumerating during a power cycle (HSD 13011253836). |
| **2.22** | PHY FW `4C08_889D`, EFI driver `0.10.06` (Intel recommends the latest from Doc ID 615203). Fixes: LAN device not enumerated after a WR cycle (#1309832919); link flaps with EEE, which OS drivers leave disabled by default (#13010560068); sporadic auto-wake during S3/S4 when AMT is provisioned (#16020921487). Adds: blocking NVM updates between I225 and I226 (#1309242132); RTD3 ULP wake from LAN_DISABLE_N negation (#1307470158); DHCP server on port 67 for AMT pre-boot network boot (#18022583990); dynamic D3Cold support at CSME's request (#1308723082). |
| **2.17** | PHY FW `4C07_888D`. |
| **2.14** | Production release. PHY FW `4C08_7877`, management FW `1.54`. EEE enabled by the Windows and Linux drivers. |
| **2.13** | Initial release. PHY FW `4C08_7877`, management FW `1.53`. Alternative MAC address section permanently removed. EEE disabled by default. |

## Disclaimer

This is an unofficial community mirror. It is not affiliated with, endorsed by or supported by Intel Corporation. The firmware images are Intel's property and are provided as-is, without warranty. Flashing NVM firmware can permanently damage your network controller, so check the controller, flash size and EtrackID before you start. Intel is a trademark of Intel Corporation or its subsidiaries.
