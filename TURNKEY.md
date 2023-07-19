# Home server/NAS (turnkey comparison)
Turnkey setups comparison

## Overview
* all solutions with 8 x 4TB storage array
* July 2023 prices without shipping
* DIY server builds **emphasized**
* X: expansion units with Time Machine backups to SATA SSD instead of M.2 or U.2
* HW: hardware without storage / S: + storage / SB: + server backup (HDD) / TMB: + Time Machine backup (SATA SSD, M.2 or U.2)

| Solution | Notes | HW | S | SB | TMB |
| :--- | :--- | ---: | ---: | ---: | ---: |
| Flashstor 12 + DAS | unRAID, 10GbE, 32GB, iGPU, bridged gen3 M.2 | 1077 | 2798 | 3317 | 3317 |
| Flashstor 12 + 4X | unRAID, 10GbE, 32GB, iGPU, bridged gen3 M.2 | 1077 | 2612 | 3422 | 3625 |
| DiskStation 8-bay + DAS | DSM, 50GbE, 64GB, no iGPU, SATA SSD | 1627 | 3407 | 3926 | 4151 |
| DiskStation 8-bay + 5X | DSM, 50GbE, 64GB, no iGPU, SATA SSD | 1627 | 3407 | 4453 | 4656 |
| Flashstor 12 + Mac Mini | unRAID+macOS, 10+20GbE, 32+8GB, 2xiGPU, bridged gen3 M.2 | 1077 | 2612 | 5066 |5066 |
| QNAP 8-bay + DAS | unRAID, 50GbE, 64GB, iGPU, SATA SSD | 3287 | 5061 | 5580 | 5790 |
| **DIY SATA budget build** | **unRAID, 50GbE, 64GB, iGPU, SATA SSD** | **2478** | **4177** | **4801** | **5793** |
| DiskStation 8-bay + Mac Mini | DSM+macOS, 50+20GbE, 64+8GB, iGPU (via Mac), SATA SSD | 1627 | 3407 | 5871 | 5871 |
| **DIY SATA build** | **unRAID, 50GbE, 128GB, iGPU, SATA SSD** | **3293** | **5027** | **5651** | **6639** |
| TerraMaster 12-bay | unRAID, 50GbE, 64GB, iGPU, SATA SSD | 4284 | 5983 | 6479 | 6832 |
| **DIY U.2 build** | **unRAID, 50GbE, 128GB, iGPU, U.2 SSD** | **4501** | **6226** | **6850** | **7838** |
| Mac Mini | macOS, 50GbE, 32GB, iGPU, U.2 SSD | 5379 | 7059 | 8060 | 8060 |

* NOTE: U.2 SSD storage solutions assume U.2 SSD prices at approx. €210 per 4TB

## Flashstor 12 + DAS
* using unRAID
* 8 x 4TB M.2 SSDs for array
* 1 x 4 TB M.2 SSD as unassigned standalone for Time Machine
* 1 x 1 TB unRAID application data cache
* NOTE: no L2ARC (RAM below 64GB)

### Stage 1
Main server + Time Machine M.2 backup

| Item  | Price |
| :--- | ---: |
| *Main hardware* | |
| Asustor Flashstor 12 Pro | 920 |
| TeamGroup Elite 32GB Kit (2 x 16GB) 3200MHz PC4-25600 CL22 TED432G3200C22DC-S01-32GB | 62 |
| *Additional hardware* | |
| 10Gb SFP+ to RJ45 10GBase-T Copper CAT.6a Transceiver Module | 61 |
| Sabrent EC-SNVE USB3.2 M.2 NVMe DAS carrier | 24 |
| 2 x SanDisk Ultra Fit 32GB | 10 |
| ————————————————————————————————————— | ——— |
| ***Subtotal*** | **1077** |
| *Storage* | |
| 9 x TeamGroup MP34 4TB gen3 M.2 NVMe SSD TM8FP4004T0C101 | 1674 |
| 1 x 1TB Samsung 980 M.2 NVMe SSD (MZ-V8V1T0BW) unRAID app data | 47 |
| ————————————————————————————————————— | ——— |
| **Total** | **2798** |

### Stage 2
Server HDD backup

| Item | Price |
| :--- | ---: |
| Icy Box IB-377U3 3.5" external enclosure | 23 |
| 22TB Seagate IronWolf Pro (ST22000NT001) HDD | 496 |
| ————————————————————————————————————— | ——— |
| **Total** | **519** |
| ————————————————————————————————————— | ——— |
| **Grand Total** | **3317** |

## Flashstor 12 + expansion
* using unRAID
* 8 x 4TB M.2 SSDs for array
* 1 x 1 TB unRAID application data cache
* NOTE: no L2ARC (RAM below 64GB)

### Stage 1
Main server

| Item  | Price |
| :--- | ---: |
| *Main hardware* | |
| Asustor Flashstor 12 Pro | 920 |
| TeamGroup Elite 32GB Kit (2 x 16GB) 3200MHz PC4-25600 CL22 TED432G3200C22DC-S01-32GB | 62 |
| *Additional hardware* | |
| 10Gb SFP+ to RJ45 10GBase-T Copper CAT.6a Transceiver Module | 61 |
| Sabrent EC-SNVE USB3.2 M.2 NVMe DAS carrier | 24 |
| 2 x SanDisk Ultra Fit 32GB | 10 |
| ————————————————————————————————————— | ——— |
| ***Subtotal*** | **1077** |
| *Storage* | |
| 8 x TeamGroup MP34 4TB gen3 M.2 NVMe SSD TM8FP4004T0C101 | 1488 |
| 1 x 1TB Samsung 980 M.2 NVMe SSD (MZ-V8V1T0BW) unRAID app data | 47 |
| ————————————————————————————————————— | ——— |
| **Total** | **2612** |

### Stage 2
Server HDD backup

| Item | Price |
| :--- | ---: |
| Asustor AS6004U 4-bay expansion | 314 |
| 22TB Seagate IronWolf Pro (ST22000NT001) HDD | 496 |
| ————————————————————————————————————— | ——— |
| **Total** | **810** |

### Stage 3
Time Machine SATA SSD backup

| Item | Price |
| :--- | ---: |
| 8 x 4TB Samsung 870 EVO SATA SSD | 203 |
| ————————————————————————————————————— | ——— |
| **Total** | **203** |
| ————————————————————————————————————— | ——— |
| **Grand Total** | **3625** |

## Synology 8-bay DiskStation + DAS
### Stage 1
Main server

| Item  | Price |
| :--- | ---: |
| *Main hardware* | |
| Synology DiskStation DS1821+ | 1050 |
| Synology E25G21-F2 (Dual 25GbE SFP28 network interface card) | 358 |
| 2 x Kingston Server Premier 32GB 2666MT/s DDR4 ECC CL19 SODIMM 2Rx8 Hynix C (KSM26SED8/32HC) | 219 |
| ————————————————————————————————————— | ——— |
| ***Subtotal*** | ***1627*** |
| *Storage* | |
| 2 x TeamGroup TM8FP44 002T0 C101 2TB M.2 NVMe SSD (r/w cache mirror) | 156 |
| 8 x 4TB Samsung 870 EVO SATA SSD | 1624 |
| ————————————————————————————————————— | ——— |
| **Total** | **3407** |

### Stage 2
Server HDD backup

| Item | Price |
| :--- | ---: |
| Icy Box IB-377U3 3.5" external enclosure | 23 |
| 22TB Seagate IronWolf Pro (ST22000NT001) HDD | 496 |
| ————————————————————————————————————— | ——— |
| **Total** | **519** |

### Stage 3
Time Machine SATA SSD backup

| Item | Price |
| :--- | ---: |
| TeamGroup MP34 4TB DRAM SLC Cache 3D NAND TLC NVMe 1.3 PCIe Gen3x4 M.2 2280 (TM8FP4004T0C101) | 186 |
| Sabrent EC-SNVE USB3.2 M.2 NVMe DAS carrier | 24 |
| CableCreation USB Type-C to USB Type-A adapter cable 1m | 15 |
| ————————————————————————————————————— | ——— |
| **Total** | **225** |
| ————————————————————————————————————— | ——— |
| **Grand Total** | **4151** |

## Synology 8-bay DiskStation + expansion
### Stage 1
Main server

| Item  | Price |
| :--- | ---: |
| *Main hardware* | |
| Synology DiskStation DS1821+ | 1050 |
| Synology E25G21-F2 (Dual 25GbE SFP28 network interface card) | 358 |
| 2 x Kingston Server Premier 32GB 2666MT/s DDR4 ECC CL19 SODIMM 2Rx8 Hynix C - KSM26SED8/32HC | 219 |
| ————————————————————————————————————— | ——— |
| ***Subtotal*** | ***1627*** |
| *Storage* | |
| 2 x TeamGroup TM8FP44 002T0 C101 2TB M.2 NVMe SSD (r/w cache mirror) | 156 |
| 8 x 4TB Samsung 870 EVO SATA SSD | 1624 |
| ————————————————————————————————————— | ——— |
| **Total** | **3407** |

### Stage 2
Server HDD backup

| Item  | Price |
| :--- | ---: |
| *Main hardware* | |
| Synology DX517 expansion unit | 460 |
| *Additional hardware* | |
| Sabrent DS-UFNC Docking Station | 90 |
| *Storage* | |
| 22TB Seagate IronWolf Pro (ST22000NT001) HDD | 496 |
| ————————————————————————————————————— | ——— |
| **Total** | **1046** |

### Stage 3
Time Machine SATA SSD backup

| Item  | Price |
| :--- | ---: |
| *Storage* | |
| 1 x 4TB Samsung 870 EVO SATA SSD (standalone Time Machine) | 203 |
|————————————————————————————————————— | ——— |
| **Total** | **203** |
| ————————————————————————————————————— | ——— |
| **Grand Total** | **4656** |

## Flashstor 12 + Mac Mini
* using unRAID
* 8 x 4TB M.2 SSDs for array
* 1 x 1 TB unRAID application data cache
* NOTE: no L2ARC (RAM below 64GB)

### Stage 1
| Item  | Price |
| :--- | ---: |
| *Main hardware* | |
| Asustor Flashstor 12 Pro | 920 |
| TeamGroup Elite 32GB Kit (2 x 16GB) 3200MHz PC4-25600 CL22 TED432G3200C22DC-S01-32GB | 62 |
| *Additional hardware* | |
| 10Gb SFP+ to RJ45 10GBase-T Copper CAT.6a Transceiver Module | 61 |
| Sabrent EC-SNVE USB3.2 M.2 NVMe DAS carrier | 24 |
| 2 x SanDisk Ultra Fit 32GB | 10 |
| ————————————————————————————————————— | ——— |
| ***Subtotal*** | **1077** |
| *Storage* | |
| 8 x TeamGroup MP34 4TB gen3 M.2 NVMe SSD TM8FP4004T0C101 | 1488 |
| 1 x 1TB Samsung 980 M.2 NVMe SSD (MZ-V8V1T0BW) unRAID app data | 47 |
| ————————————————————————————————————— | ——— |
| **Total** | **2612** |

### Stage 2
Mac Mini: Time Machine M.2 & server HDD backup

| Item  | Price |
| :--- | ---: |
| *Hardware* | |
| Mac Mini M2 8GB 256 GB | 699 |
| SonnetTech Twin10G SFP+ | 764 |
| OWC miniStack STX | 283 |
| *Additional hardware* | |
| Anker Thunderbolt cable 70cm (DAS) | 36 |
| *Storage* | |
| 22TB Seagate IronWolf Pro (ST22000NT001) HDD | 496 |
| TeamGroup MP34 4TB gen3 M.2 NVMe SSD TM8FP4004T0C101  | 186
|————————————————————————————————————— | ——— |
| **Total** | **2454** |
| ————————————————————————————————————— | ——— |
| **Grand Total** | **5066** |

## QNAP 8-bay + DAS
* using unRAID

### Stage 1
Main server

| Item  | Price |
| :--- | ---: |
| *Main hardware* | |
| QNAP TVS-h874 | 2725 |
| 2 x Kingston 32GB DDR4 3200MT/s Non-ECC Unbuffered SODIMM (KVR32S22D8/32) | 126 |
| *Additional hardware* | |
| QNAP QXG-25G2SF-CX6 dual SFP28 | 431 |
| SanDisk Ultra Fit 32GB | 5 |
| ————————————————————————————————————— | ——— |
| ***Subtotal*** | **3287** |
| *Storage* | |
| 8 x 4TB Samsung 870 EVO SATA SSD | 1624 |
| 1 x 250GB Samsung 980 PRO M.2 NVMe SSD (MZ-V8P250BW) L2ARC/MD | 85 |
| 1 x 1TB Samsung 980 PRO M.2 NVMe SSD (MZ-V8P1T0BW) unRAID app data | 65 |
| ————————————————————————————————————— | ——— |
| **Total** | **5061** |

### Stage 2
Server SATA HDD USB3 (A) backup

| Item | Price |
| :--- | ---: |
| Icy Box IB-377U3 3.5" external enclosure | 23 |
| 22TB Seagate IronWolf Pro (ST22000NT001) HDD | 496 |
| ————————————————————————————————————— | ——— |
| **Total** | **519** |

### Stage 3
Time Machine M.2 USB-C backup

| Item | Price |
| :--- | ---: |
| TeamGroup MP34 4TB DRAM SLC Cache 3D NAND TLC NVMe 1.3 PCIe Gen3x4 M.2 2280 (TM8FP4004T0C101) | 186 |
| Sabrent EC-SNVE USB3.2 M.2 NVMe DAS carrier | 24 |
| ————————————————————————————————————— | ——— |
| **Total** | **210** |
| ————————————————————————————————————— | ——— |
| **Grand Total** | **5790** |

## Synology 8-bay DiskStation + Mac Mini
### Stage 1
Main server

| Item  | Price |
| :--- | ---: |
| *Main hardware* | |
| Synology DiskStation DS1821+ | 1050 |
| Synology E25G21-F2 (Dual 25GbE SFP28 network interface card) | 358 |
| 2 x Kingston Server Premier 32GB 2666MT/s DDR4 ECC CL19 SODIMM 2Rx8 Hynix C - KSM26SED8/32HC | 219 |
| ————————————————————————————————————— | ——— |
| ***Subtotal*** | **1627** |
| *Storage* | |
| 2 x 2TB TeamGroup TM8FP44 002T0 C101 M.2 NVMe SSD (r/w cache mirror) | 156 |
| 8 x 4TB Samsung 870 EVO SATA SSD | 1624 |
| ————————————————————————————————————— | ——— |
| **Total** | **3407** |

### Stage 2
Mac Mini: Time Machine M.2 & server HDD backup + media server

| Item  | Price |
| :--- | ---: |
| *Hardware* | |
| Mac Mini M2 8GB 256 GB | 699 |
| SonnetTech Twin10G SFP+ | 764 |
| OWC miniStack STX | 283 |
| *Additional hardware* | |
| Anker Thunderbolt cable 70cm (DAS) | 36 |
| *Storage* | |
| 22TB Seagate IronWolf Pro (ST22000NT001) HDD | 496 |
| TeamGroup MP34 4TB gen3 M.2 NVMe SSD TM8FP4004T0C101  | 186
|————————————————————————————————————— | ——— |
| **Total** | **2454** |
| ————————————————————————————————————— | ——— |
| **Grand Total** | **5871** |

## TerraMaster 12-bay
* using unRAID
* Intel Core i3-9100

### Stage 1
Main server

| Item  | Price |
| :--- | ---: |
| *Main hardware* | |
| TerraMaster U12-322-9100 (estimate) | 3600 |
| 4 x Kingston ValueRAM 16GB 2666MT/s DDR4 Non-ECC CL19 DIMM 1Rx8 (KVR26N19S8/16) | 140 |
| *Additional hardware* | |
| Intel XXV710-DA2 dual 25GbE SFP28 | 296 |
| Delock 9035 PCIe 3.0 x8 dual M.2 card | 248 |
| ————————————————————————————————————— | ——— |
| ***Subtotal*** | **4284** |
| *Storage* | |
| 8 x 4TB Samsung 870 EVO SATA SSD | 1624 |
| 1 x 250GB Samsung 980 M.2 NVMe SSD (MZ-V8V250BW) L2ARC/MD | 28 |
| 1 x 1TB Samsung 980 M.2 NVMe SSD (MZ-V8V1T0BW) unRAID app data | 47 |
| ————————————————————————————————————— | ——— |
| **Total** | **5983** |

### Stage 2
Server backup

| Item | Price |
| :--- | ---: |
| 22TB Seagate IronWolf Pro (ST22000NT001) HDD | 496 |
| ————————————————————————————————————— | ——— |
| **Total** | **496** |

### Stage 3
Time Machine SATA SSD backup

| Item | Price |
| :--- | ---: |
| 1 x 4TB Samsung 870 EVO SATA SSD | 203 |
| ————————————————————————————————————— | ——— |
| **Total** | **203** |

### Stage 4
Additional M.2 NVMe

| Item | Price |
| :--- | ---: |
| 1 x 2TB Sabrent Rocket gen3 SB-ROCKET-2TB | 150 |
| ————————————————————————————————————— | ——— |
| **Total** | **150** |
| ————————————————————————————————————— | ——— |
| **Grand Total** | **6832** |

## Mac Mini
### Stage 1
Main server

| Item  | Price |
| :--- | ---: |
| *Main hardware* | |
| Mac Mini M2 Pro 32GB 1TB | 2239 |
| SonnetTech Twin25G | 1042 |
| 2 x OWC Flex 1U4 | 2098 |
| ————————————————————————————————————— | ——— |
| ***Subtotal*** | **5379** |
| *Storage* | |
| 8 x Intel DC P4510 2.5" 4TB U.2 NVMe SSD | 1680 |
| ————————————————————————————————————— | ——— |
| **Total** | **7059** |

### Stage 2
Time Machine M.2 & server HDD backup

| Item  | Price |
| :--- | ---: |
| *Hardware* | |
| OWC miniStack STX | 283 |
| *Additional hardware* | |
| Anker Thunderbolt cable 70cm (DAS) | 36 |
| *Storage* | |
| 22TB Seagate IronWolf Pro (ST22000NT001) HDD | 496 |
| TeamGroup MP34 4TB gen3 M.2 NVMe SSD TM8FP4004T0C101  | 186
|————————————————————————————————————— | ——— |
| **Total** | **1001** |
| ————————————————————————————————————— | ——— |
| **Grand Total** | **8060** |
