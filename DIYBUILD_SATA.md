# Home server/NAS (SATA build)
DIY NAS/server build for unRAID or TrueNAS Scale with SATA SSDs for main storage array

## Overview
### Total prices
| Item  | Price |
| :--- | ---: |
| Stage 1 (main) | 5027 |
| Stage 2 (backup) | 624 | 
| Stage 3 (Time Machine) | 988 |
| ———————————————— | ——— |
| **Grand Total** | **6639** |

### Prices
July 2023 prices without shipping

#### Stage 1
Fundamental server setup

| Item  | Price |
| :--- | ---: |
| *Chassis hardware* | |
| Main rackmount  | 210 |
| Slide rails  | 70 |
| Internal cage | 23 |
| 8 x 2.5" SATA array backplane | 246 |
| USB dust plugs | 30 |
| *Cables* | |
| Slim SAS to Mini SAS | 61 |
| Mini SAS to 4 x SATA reverse | 29 |
| SATA + SATA power (Y) | 8 |
| Low Noise Adapters | 4 |
| *Fans* | |
| 3 x 80mm PWM | 54 |
| 2 x 50mm | 13 |
| *Additional chassis devices* | |
| Optical drive | 81 |
| *Main hardware* | |
| Mainboard | 502 |
| CPU | 618 |
| CPU cooler | 70 |
| 128 GB ECC DDR5 RAM | 500 |
| Dual SFP28 network card | 376 |
| PSU | 220 |
| *Additional hardware* |
| PCIe 3.0 x1 SATA card | 40 |
| *Storage hardware* | |
| USB header adapter | 10 |
| USB to mSATA adapter | 18 |
| mSATA SSD | 110 |
| ———————————————— | ——— |
| ***Subtotal*** | ***3293*** |
| *Storage* | |
| 8 x 4TB SATA SSD | 1624 |
| 500GB gen4 M.2 SSD (L2ARC) | 45 |
| 1TB gen4 M.2 SSD (unRAID cache) | 65 |
| ———————————————— | ——— |
| **Total** | **5027** |

#### Stage 2
Server HDD backup

| Item  | Price |
| :--- | ---: |
| *Chassis hardware* |
| HDD cage backplane | 72 |
| *Cables* | |
| SATA to Molex power | 4 |
| SATA | 3 |
| *Fans* | |
| 1 x 40x10mm fan | 14 |
| *Additional hardware* | |
| HDD docking station | 35 |
| *Storage* | |
| 22TB HDD | 496 |
| ———————————————— | ——— |
| **Total** | **624** |

#### Stage 3
Time Machine U.2 backup

| Item  | Price |
| :--- | ---: |
| *Chassis hardware* | |
| Quad U.2 cage backplane | 472 |
| *Cables* | |
| OCuLink | 74 |
| *Fans* | |
| 2 x 40x20mm fan | 28 |
| *Additional hardware* | |
| PCIe 4.0 x4 U.2 card | 40 |
| U.2 docking station | 164 |
| *Storage* | |
| 4TB U.2 NVMe SSD | 210 |
| ———————————————— | ——— |
| **Total** | **988** |

#### Optional hardware

| Item  | Price |
| :--- | ---: |
| *Chassis hardware* | |
| PCIe expansion holder | 17  |
| *Main hardware* | |
| Mainboard IPMI version (add. cost) | 80 |
| ———————————————— | ——— |
| **Total** | **97** |

### Maximum power consumption
n/a

## Chassis hardware
4U modular rackmount

### SilverStone RM41-506
* 4U 6-bay 5.25" rackmount server
* 430mm (W) x 176mm (H) x 446mm (D) / max card length: 278mm / max CPU cooler height: 148mm
* https://www.silverstonetek.com/en/product/info/computer-chassis/RM41-506/
* Price: 210

### Additional chassis hardware
#### SilverStone RMS06-22
* Set of 2 x server chassis slide rails
* https://www.silverstonetek.com/en/product/info/server-nas/RMS06-22/
* Price: 70

#### SilverStone G11909520-RT
* PCIe expansion card holder
* https://www.silverstonetek.com/en/product/info/server-nas/G11909520-RT/
* NOTE: only needed for full-height cards, e.g. quad M.2 carrier cards
* Price: 17

#### SilverStone G11909510-RT
* 4 x 3.5" & 1 x 2.5" cage for internal drives (center)
* https://www.silverstonetek.com/en/product/info/server-nas/G11909510-RT/
* Price: 23

#### RaidSonic Icy Box IB-2281SAS-12G
* Dual 5.25" cage with backplane for 8 x 2.5" SATA SSD drives (lower right)
* https://icybox.de/en/interne_speicherloesungen/IB-2281SAS-12G
* Fans: 2 x 50x??mm (50x10?)
* Price: 246

#### Icy Dock DataCage Basic MB876SK-B
* 5.25" cage with backplane for 1 x 3.5" SATA HDD (lower left)
* https://global.icydock.com/product_35.html
* Molex power input
* Fans 1 x 40x10mm
* NOTE: used for 3.5" SATA HDD (server backup)
* Price: 72

#### Icy Dock ToughArmor MB699VP-B V3
* 5.25" cage with backplane for 4 x 2.5" U.2 NVMe SSDs (upper right)
* https://global.icydock.com/product_326.html
* NOTE: used for 1 x U.2 (Time Machine backup)
* OCuLink connector / tri-mode compatible
* Fans: 2 x 40x20mm
* Price 472

#### 10 x USB Type-A dust plug
* 7 x rear, 1 x internal, 2 x front
* https://www.amazon.de/dp/B00NOK1GXI/
* Price: 30 (10 x 3)

#### Cables
##### SATA power to Molex power
* Delock 60140 Power Cable SATA 15 pin male > 4 pin female 100 cm
* https://www.delock.de/produkt/60140/merkmale.html?setLanguage=en
* Price: 4

##### Slim SAS to Mini SAS
* Slim SAS 4i SFF-8654 38-pin host to 1 x Mini SAS SFF-8643 target adapter cable
* InLine Slim SAS Cable SFF-8654 to Mini SAS HD SFF-8643, 24Gb/s, 1m 
* https://www.kabelprofishop.de/nfl19045/inline-slim-sas-kabel-sff-8654-zu-mini-sas-hd-sff-8643-24gb/s-1m
* Price: 61

##### Mini SAS to 4 x SATA reverse
* Mini SAS to 4 x SATA reverse breakout cable
* Delock 83320 Cable Mini SAS HD SFF-8643 > 4 x SATA 7 pin Reverse + Sideband 0.5 m
* https://www.delock.com/produkt/83320/merkmale.html?setLanguage=en
* NOTE: used for 4 x SATA SSDs / sideband only for hardware RAID
* Price: 29

##### 1 x SATA
* Delock 82809 SATA 6 Gb/s Cable 50 cm yellow
* https://www.delock.de/produkt/82809/merkmale.html?setLanguage=en
* NOTE: used for backup HDD
* Price: 3

##### 22-pin SATA Y-cable
* Delock 85228 Cable SATA 6 Gb/s 7 pin receptacle + SATA 15 pin power plug > SATA 22 pin receptacle straight metal 30 cm
* https://www.delock.de/produkt/85228/merkmale.html?setLanguage=en
* NOTE: used for optical drive
* Price: 8

##### OCuLink
* Delock 85214 Cable OCuLink PCIe SFF-8611 to OCuLink SFF-8611 1 m
* https://www.delock.de/produkt/85214/merkmale.html?setLanguage=en
* NOTE: used for connecting to U.2 backplane (Time Machine backup)
* Price: 74

#### Fans
##### General
* 3 x 80x25mm (PWM)
* 2 x 50x??mm (50x10?)
* 2 x 40x20mm
* 1 x 40x10mm

##### 3 x 80x25mm (PWM)
* 2 x back (main chassis) / 1 x front center (G11909510-RT)
* 3 x Noctua NF-A8 PWM (80x80x25, 4-pin PWM 12V / with LNA: 450–1750rpm, 13.8dB)
* https://noctua.at/en/nf-a8-pwm/specification
* NOTE: LNA included
* Power (max): 2.88W (3 x 0.96W)
* Price: 54 (3 x 18)

##### 2 x 50x10mm
* for IB-2281SAS-12G
* 2 x AABCooling Super Silent Fan 5 (50x50x11, 3-pin 12 V / 3500 rpm, 17.5dB)
* https://www.aabcooling.de/product-eng-43-AABCOOLING-Super-Silent-Fan-5.html
* Power: n/a (via SATA, max: 0.6W x 2 = 1.2W)
* Price: 13 (2 x 6.50)

##### 2 x 40x20mm
* for MB699VP-B V3
* Noctua NF-A4x20 FLX (40x40x20, 3-pin 12V / with ULNA: 3700rpm, 8.5dB)
* https://noctua.at/en/products/fan/nf-a4x20-flx
* NOTE: LNA & ULNA included
* Power: n/a (via SATA, max: 0.6W x 2 = 1.2W)
* Price 28 (2 x 14)

##### 1 x 40x10mm
* for DataCage Basic MB876SK-B
* Noctua NF-A4x10 FLX (40x40x10, 3-pin 12V / with LNA: 3700rpm, 12.9dB)
* https://noctua.at/en/nf-a4x10-flx/specification
* NOTE: LNA included
* Power: n/a (via SATA, max: 0.6W)
* Price: 14

##### 2 x 3-pin low-noise adapters
* for 50mm fans
* Noctua NA-SRC10
* https://noctua.at/en/na-src10/specification
* Price: 4 (2 x 2)

### Additional chassis devices
#### CD/DVD/BD optical drive
* for use with MakeMKV and Ripper on unRAID
* upper left 5.25" bay
* Asus BW-16D1HT with UHD-friendly firmware
* https://www.asus.com/uk/motherboards-components/optical-drives/internal-blu-ray-drive/bw16d1ht/
* Power (max): 30W (54W via SATA)
* Price: 81

## Main hardware
### Motherboard
* ASUS Pro WS W680-ACE workstation mainboard
* CPU: PCIe 5.0 (16/8+8), PCIe 4.0 (x4 M.2), DDR5 ECC (128GB)
* https://www.asus.com/motherboards-components/motherboards/workstation/pro-ws-w680-ace/techspec/
* OPTIONAL: IPMI version / alternative: TinyPilot Voyager 2a
* Power (max, high-end boards): 80W
* Price: 502 (582 + IPMI)

#### PCH
* Intel W680
* https://www.anandtech.com/show/17308/the-intel-w680-chipset-overview-ecc-for-alder-lake-workstations
* https://ark.intel.com/content/www/us/en/ark/products/218834/intel-w680-chipset.html
* DMI speed: PCIe 4.0 x8 (8 x x1, 15.754 GB/s = 126 Gb/s)
* PCIe lanes: 12 x 4.0, 16 x 3.0 (39.388 GB/s = 315 Gb/s)
* 4 x SATA direct, Slim SAS (4 x SATA or PCIe 4.0 x4 mode)
* 8 x SATA max read speed with RAID-Z2 via PCH: 4.48 GB/s
* 3 x PCIe: 2 x PCIe 3.0 x4 (x16 physical), 1 x PCIe 3.0 x1
* 2 x M.2 (PCIe 4.0 x4)
* Thunderbolt 4 & USB3.2 2x2 headers

### CPU
* iGPU / PCI 5.0 / DDR5 / ECC / 35W TDP
* Intel Core i9-13900T 1.1 GHz 24-Core OEM/Tray Processor
* https://ark.intel.com/content/www/us/en/ark/products/230498/intel-core-i913900t-processor-36m-cache-up-to-5-30-ghz.html
* Power (max, turbo): 106W
* NOTE: reduce power (undervolt, disable TurboBoost & HyperThreading etc.)
* Price: 618

#### CPU cooler
* maximum height: 148mm
* Noctua NH-U9S (LGA1700 & LGA1151 / 93W TDP max / 4-pin PWM 12V / with LNA: 450–1550rpm, 16.3dB max)
* https://noctua.at/en/nh-u9s/specification
* NOTE: LNA included
* Power (max, fan): 1.2W
* Price: 70

### RAM
* 128GB DDR5 ECC 4400 MHz
* 4 x Crucial Micron 32GB DDR5-4800 ECC UDIMM 2Rx8 CL40 (MTC20C2085S1EC48BA1R)
* https://www.crucial.com/memory/server-ddr5/mtc20c2085s1ec48br
* Power: 48W (3W per 8GB)
* Price 500 (4 x 125)

### Network interface card
* Dual 25GbE SFP28 adapter card (gen4)
* 10Gtek E810-25G-2S-X8 (PCIe 4.0 x8)
* PCIe speed: 15.754 GB/s = 126 Gb/s
* NIC speed: 6.25 GB/s = 50 Gb/s
* https://www.sfpcables.com/25g-network-card-dual-sfp28-port-inter-e810-xxvam2-controller-x8-lane
* Power (max): 20.8W (75W max via PCIe)
* Price: 376

## Additional hardware

### Auxiliary SATA storage card
* for use with optical drive and hotswap HDD backup drive
* Delock 90010 PCIe 3.0 x1 4-port SATA III card
* https://www.delock.de/produkt/90010/merkmale.html?setLanguage=en
* Chipset: Asmedia ASM1064
* NOTE: effective 2-port with only one lane active at a time
* Power (max, x1): 10W
* Price: 40

### OCuLink PCIe adapter card
* for use with Time Machine backups (in PCIe 3.0 x4 slot)
* Delock 90482 PCI Express 4.0 x4 Card to 1 x internal OCuLink SFF-8612
* PCIe speed: 3.938 GB/s = 31.504 Gb/s
* https://www.delock.de/produkt/90482/merkmale.html?setLanguage=en
* Price: 40

## Storage hardware
### OS boot drive
DIY USB3/mSATA DOM (internal on motherboard)

#### 20-pin USB3 header USB3 Type A adapter 
* Delock 41865 USB 3.0 Pin Header female > 2 x USB 3.0 female – up, stacked
* https://www.delock.de/produkt/41865/merkmale.html?setLanguage=en
* Price: 10

#### USB3.0 mSATA Adapter
* Delock 62681 Converter USB 5 Gbps Type-A male > mSATA full size (76mm)
* https://www.delock.de/produkt/62681/merkmale.html?setLanguage=en
* NOTE: two adapters for TrueNAS Scale (mirror)
* Power (max, USB3): 4.5W
* Price: 18 (36 for TrueNAS Scale)

#### 256GB mSATA SSD (MLC NAND)
* Transcend 256GB SATA III 6Gb/s MSA370S mSATA SSD 370S (TS256GMSA370S)
* https://www.amazon.de/dp/B08BXF8KS2
* NOTE: two SSDs for TrueNAS Scale (mirror)
* Power (max, cheap mSATA brands): 2W (4W for TrueNAS Scale)
* Price: 110 (220 for TrueNAS Scale)

### PCIe 4.0 x4 M.2 SSDs
#### 500GB (CPU-direct)
* for ZFS L2ARC metadata-only read cache
* Samsung 980 PRO 500GB M.2 NVMe SSD (MZ-V8P500BW), write 5000 MB/s, read: 6900 MB/s
* https://www.samsung.com/us/computing/memory-storage/solid-state-drives/980-pro-pcie-4-0-nvme-ssd-500gb-mz-v8p500b-am/
* Power: 6W
* Price: 45

#### 1TB (via PCH)
* for unRAID application data cache
* 1TB Samsung 980 PRO M.2 NVMe SSD (MZ-V8P1T0BW)
* https://www.samsung.com/us/computing/memory-storage/solid-state-drives/980-pro-pcie-4-0-nvme-ssd-1tb-mz-v8p1t0b-am/
* Power: 6W
* Price: 65 

### 8 x 4TB SATA SSDs
* main storage array (RAID-Z2)
* 8 x 4TB Samsung 870 EVO SATA III 2.5 inch SSD (MZ-77E4T0B/EU)
* NOTE: 32TB raw, 24TB usable, 19.2TB effective (80%)
* Power: n/a (via SATA, max: 20.64W = 8 x 2.58W)
* Price: 1624 (8 x 203)

### U.2 NVMe SSD
* PCIe 3.0 x4 for Time Machine backup (standalone unassigned ext4 drive)
* Intel DC P4510 2.5" 4TB
* https://www.storagereview.com/review/intel-ssd-dc-p4510-review
* Power: 14W
* Price: 210

### SATA HDD
* for server content backups (standalone unassigned ext4 drive)
* 22TB Seagate IronWolf Pro (ST22000NT001)
* https://www.seagate.com/products/nas-drives/ironwolf-hard-drive/
* NOTE: 512MB buffer
* Power: n/a (via SATA, max: 8W)
* Price: 496

## PSU
### General considerations
* PSU capacity as close to twice of maximum server load
* e.g.: server at 500W max means PSU at 1000W for best efficiency
* Titanium / tier 1

### 850W 80+ Titanium PSU
* BeQuiet! Dark Power 13 850W
* https://www.bequiet.com/en/powersupply/4043
* Price: 220

## Unused options for hardware expansion
* PCIe 5.0 x8 (CPU direct)
* PCIe 3.0 x4 (PCH)
* 1 x PCIe 4.0 x4 M.2 NVMe (PCH)

### Options
* 1 x PCIe 4.0 x4 M.2 NVMe for additional unRAID cache
* PCIe 5.0 x8: PCIe 4.0 x8 card for 4 x gen3 U.2 or M.2 high-speed storage array (for iSCSI)
* PCIe 3.0 x4 or 5.0 x8: SAS HBA for JBOD (needs SAS Expander)

## External hardware
### RaidSonic Icy Box IB-1121-C31 (USB-C)
* HDD docking station as macOS DAS for server backup direct access
* https://icybox.de/en/product.php?id=181
* NOTE: Paragon extFS for Mac needed
* Price: 35

### Icy Dock EZ-Adapter Ex MB931U-1VB
* U.2 docking station (USB-C/TB) as macOS DAS for Time Machine direct access
* https://global.icydock.com/product_288.html
* NOTE: Paragon extFS for Mac needed
* Price: 164
