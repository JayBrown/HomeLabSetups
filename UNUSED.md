# Home server/NAS (unused hardware solutions)
DIY NAS/server build for unRAID or TrueNAS Scale: unused hardware solutions

## Boot drive
### OS boot drive
DIY USB3/mSATA DOM (internal on motherboard)

* NOTE: dual setup for mirrored boot volume on TrueNAS Scale
* NOTE (unRAID): 32GB max, USB, no mirror

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