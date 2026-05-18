# Intel I225-V / I226-V NVM Firmware
Firmware files for the Intel I225-V and I226-V network controllers, available in 1MB and 2MB versions.

---

### I225-V
| 1MB File Name               | Ver | EtrackID | 2MB File Name               | Ver | EtrackID |
|-----------------------------|-----|----------|-----------------------------|-----|----------|
| `FXVL_15F3_V_1MB_1.45.bin`  |1.45 | 80000150 | `FXVL_15F3_V_2MB_1.45.bin`  |1.45 | 8000014B |
| `FXVL_15F3_V_1MB_1.57.bin`  |1.57 | 80000182 | `FXVL_15F3_V_2MB_1.57.bin`  |1.57 | 80000185 |
| `FXVL_15F3_V_1MB_1.68.bin`  |1.68 | 800001CE | `FXVL_15F3_V_2MB_1.68.bin`  |1.68 | 800001C7 |
| `FXVL_15F3_V_1MB_1.89.bin`  |1.89 | 800002FC | `FXVL_15F3_V_2MB_1.89.bin`  |1.89 | 800002F4 |
|                             |     |          |                             |     |          |

---

### I226-V
| 1MB File Name               | Ver | EtrackID | 2MB File Name               | Ver | EtrackID |
|-----------------------------|-----|----------|-----------------------------|-----|----------|
| `FXVL_125C_V_1MB_2.14.bin`  |2.14 | 80000290 | `FXVL_125C_V_2MB_2.14.bin`  |2.14 | 8000028D |
| `FXVL_125C_V_1MB_2.17.bin`  |2.17 | 80000308 | `FXVL_125C_V_2MB_2.17.bin`  |2.17 | 80000303 |
| `FXVL_125C_V_1MB_2.23.bin`  |2.23 | 8000039D | `FXVL_125C_V_2MB_2.22.bin`  |2.22 | 80000371 |
| `FXVL_125C_V_1MB_2.27.bin`  |2.27 | 80000425 | `FXVL_125C_V_2MB_2.25.bin`  |2.25 | 800003AD |
| `FXVL_125C_V_1MB_2.32.bin`  |2.32 | 80000425 | `FXVL_125C_V_2MB_2.27.bin`  |2.27 | 80000422 |
|                             |     |          | `FXVL_125C_V_2MB_2.32.bin`  |2.32 | 80000422 |

### I226-V Release Notes

| Version | Onboard I226-V |
|---------|----------------|
| 2.32 | Fixes an issue in MDI lane swap handling that caused the P (positive) and N (negative) signal polarities to be swapped incorrectly. |
| 2.27 | **General Note:**<br>1. PHY FW: 4C08_88B6<br>2. EFI LAN driver in 2MB: 0.10.06<br><br>**Bug Fix:**<br>• HSD 13012034657: [Foxville][NVM] QV Tools External Loopback test fails with NVM version 2.25 |
| 2.25 | **General Note:**<br>1. PHY FW: 4C08_08a6<br>2. EFI LAN driver in 2MB: 0.10.06<br><br>**Bug Fix:**<br>• HSD 13010560068: Link Flaps with Energy Efficient Ethernet Enabled<br>• HSD 13011274310: Unexpected Link |
| 2.23 | **General Note:**<br>1. PHY FW: 4C08_889D<br>2. EFI LAN driver in 2MB: 0.10.06<br><br>**Bug Fix:**<br>• HSD 13011253836: Device Not Enumerated during power cycle (restart, power-on, etc.) |
| 2.22 | 1. Update PHY FW to 4C08_889D<br>2. EFI LAN driver: 0.10.06 (recommend to update to the latest version in Doc ID: 615203).<br><br>**Bug Fix:**<br>• #1309832919: LAN Device not enumerated after WR cycle<br>• #13010560068: Link flaps with Energy Efficient Ethernet<br>&nbsp;&nbsp;o Note: Energy Efficient Ethernet Setting is controlled by OS drivers for both Windows and Linux and the default setting is Disabled.<br>• #16020921487: [AMT provisioned] Sporadically Autowake during S3/S4<br><br>**RCR:**<br>• #1309242132: Prevent NVM update between I225 and I226<br>• #1307470158: Enable RTD3 ULP wake from LAN_DISABLE_N negation<br>• #18022583990: [AMT provisioned] Enable DHCP server (port 67) for PreBoot Network Boot Support<br>• #1308723082: Dynamic D3Cold support for preventing D3Cold in S0 upon request from CSME |
| 2.17 | 1. Update PHY FW to 4C07_888D |
| 2.14 | **Production Release**<br>1. PHY FW to 4C08_7877<br>2. Management FW: 1.54<br>3. Energy Efficient Ethernet is enabled by the driver (Windows & Linux) |
| 2.13 | **Initial Release**<br>1. PHY FW to 4C08_7877<br>2. Management FW: 1.53<br>3. Alternative MAC address section is permanently removed<br>4. Energy Efficient Ethernet is disabled by default |

