# Home server/NAS (SATA budget build)
DIY NAS/server budget build for unRAID or TrueNAS Scale with SATA SSDs for main storage array

## Overview
### Total prices
| Item  | Price |
| :--- | ---: |
| Stage 1 (main) | 4177 |
| Stage 2 (backup) | 624 | 
| Stage 3 (Time Machine) | 992 |
| ———————————————— | ——— |
| **Grand Total** | **5793** |

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
| SATA + SATA power (Y) | 8 |
| Low Noise Adapters | 4 |
| *Fans* | |
| 3 x 80mm PWM | 54 |
| 2 x 50mm | 13 |
| *Additional chassis devices* | |
| Optical drive | 81 |
| *Main hardware* | |
| Mainboard | 279 |
| CPU | 200 |
| CPU cooler | 70 |
| 64 GB ECC DDR4 RAM | 248 |
| Dual SFP28 network card | 296 |
| PSU | 220 |
| *Additional hardware* |
| PCIe 3.0 x4 dual M.2 carrier card | 248 |
| PCIe 3.0 x1 SATA card | 40 |
| *Storage hardware* | |
| USB header adapter | 10 |
| USB to mSATA adapter | 18 |
| mSATA SSD | 110 |
| ———————————————— | ——— |
| ***Subtotal*** | ***2478*** |
| *Storage* | |
| 8 x 4TB SATA SSD | 1624 |
| 256GB gen3 M.2 SSD (L2ARC) | 28 |
| 1TB gen3 M.2 SSD (unRAID cache) | 47 |
| ———————————————— | ——— |
| **Total** | **4177** |

#### Stage 2
Server HDD backup

| Item  | Price |
| :--- | ---: |
| *Chassis hardware* |
| 1 x HDD cage backplane | 72 |
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
| PCIe 3.0 x4 OCuLink card | 44 |
| U.2 docking station | 164 |
| *Storage* | |
| 4TB U.2 NVMe SSD | 210 |
| ———————————————— | ——— |
| **Total** | **992** |

#### Optional hardware

| Item  | Price |
| :--- | ---: |
| *Chassis hardware* | |
| PCIe expansion holder | 17  |
| ———————————————— | ——— |
| **Total** | **17** |

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
* Asus WS 246 Pro workstation mainboard
* CPU: PCIe 3.0 (16/8+8), DDR4, ECC / via PCH: 8 x SATA, 1 x M.2 x4, 1 x M.2 x2 (shared with SATA), 3 x USB headers (2x2.0, 1x3.0)
* https://www.asus.com/motherboards-components/motherboards/workstation/ws-c246-pro/techspec/
* Power (estimate): 60W
* Price: 279

#### PCH
* Intel C246
* https://ark.intel.com/content/www/us/en/ark/products/147326/intel-c246-chipset.html
* DMI speed: PCIe 3.0 x4 (4 x x1, 3.938 GB/s = 31.5 Gb/s)
* PCIe lanes: 24 x 3.0 (effective: 4 x 3.0)
* 8 x SATA = PCIe 3.0 x4
* SATA max read speed at RAID-Z2: 4.48 GB/s (effective: 3.938 GB/s
* NOTE: DMI will be the bottleneck
* 1 x PCIe 3.0 x1 for auxiliary 2-port SATA
* 1 x PCIe 3.0 x4 (x16 physical) for OCuLink to U.2

### CPU
* iGPU / PCIe 3.0 / DDR4 / ECC / 35W TDP
* Intel Core i3-9100T 4-core OEM/Tray Processor (1151)
* 16 x PCIe 3.0: up to 1x16, 2x8, 1x8+2x4)
* https://ark.intel.com/content/www/us/en/ark/products/134871/intel-core-i39100t-processor-6m-cache-up-to-3-70-ghz.html
* Power (max, estimate): 50W
* NOTE: if possible, reduce power (undervolt, disable TurboBoost & HyperThreading etc.)
* Price (new, import, minimum): 200

#### CPU cooler
* maximum height: 148mm
* Noctua NH-U9S (LGA1700 & LGA1151 / 93W TDP max / 4-pin PWM 12V / with LNA: 450–1550rpm, 16.3dB max)
* https://noctua.at/en/nh-u9s/specification
* NOTE: LNA included
* Power (max, fan): 1.2W
* Price: 70

### RAM
* 64GB DDR4 ECC 2400 MHz (1Rx8, single rank)
* 4 x 16GB Kingston DDR4 2666MT/s ECC Unbuffered RAM Memory DIMM (KSM26ED8: 16MF; optional: 16HC)
* https://www.kingstonmemoryshop.co.uk/motherboard/asus/ws-series/asus-ws-c246-pro-motherboard?filter=1602,556,91
* Power: 24W (3W per 8GB)
* Price: 248 (4 x 62)

### Network interface card
* Dual 25GbE SFP28 adapter card (gen3)
* Intel XXV710-DA2 (PCIe 3.0 x8)
* PCIe speed: 7.877 GB/s = 63 Gb/s
* NIC speed: 6.25 GB/s = 50 Gb/s
* https://ark.intel.com/content/www/us/en/ark/products/95260/intel-ethernet-network-adapter-xxv710da2.html
* Power (max): XXX (75W max via PCIe)
* Price: 296

## Additional hardware
### M.2 NVMe SSD carrier card (PLX)
* for use as cache drives (L2ARC & unRAID application data)
* Delock 90305 PCI Express x8 Card to 2 x internal NVMe M.2 Key M
* https://www.delock.de/produkt/90305/merkmale.html?setLanguage=en
* Power (max): ???
* Price: 248

### Auxiliary SATA storage card
* for use with optical drive and hotswap HDD backup drive
* Delock 90010 PCIe 3.0 x1 4-port SATA III card
* https://www.delock.de/produkt/90010/merkmale.html?setLanguage=en
* Chipset: Asmedia ASM1064
* NOTE: effective 2-port with only one lane active at a time
* Power (max, x1): 10W
* Price: 40

### OCuLink PCIe adapter card
* for use with Time Machine backups
* Delock 90307 PCI Express 3.0 x4 Card to 1 x internal OCuLink SFF-8612
* https://www.delock.de/produkt/90307/merkmale.html?setLanguage=en
* Price: 44

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

### PCIe 3.0 x4 M.2 SSDs
#### 256GB
* for ZFS L2ARC metadata-only read cache
* Samsung 980 256GB M.2 NVMe SSD (MZ-V8V250BW), write 1300 MB/s, read: 2900 MB/s
* https://www.samsung.com/us/computing/memory-storage/solid-state-drives/980-pcie-3-0-nvme-gaming-ssd-250gb-mz-v8v250b-am/
* Power: 6W
* Price: 28

#### 1TB
* for unRAID application data cache
* 1TB Samsung 980 M.2 NVMe SSD (MZ-V8V1T0BW), write 3000 MB/s, read 3500 MB/s
* https://www.samsung.com/sg/memory-storage/nvme-ssd/980-1tb-nvme-pcie-gen-3-mz-v8v1t0bw/
* Power: 6W
* Price: 47 

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
* 1 x M.2 (PCIe 3.0 x4); alternative: M.2 via CPU-direct carrier card

### Options
* additional cache drive

### Expansion not for use
* 1 x PCIe 3.0 x4 (x16 physical; real electrical: x2, PCIEX16_4 shared with 4 x SATA)
* 1 x M.2 (PCIe 3.0 x4; real: x2, shared with 4 x SATA)

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
