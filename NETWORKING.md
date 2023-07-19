# Home lab
Home lab network setup

## Overview
### Total prices
| Item  | Price |
| :--- | ---: |
| Stage 1 (main hardware) | 1933 |
| Stage 2 (UPS & Mini-PC) | 956 | 
| Stage 3 (TinyPilot & Dual SFP28) | 1237 |
| ———————————————— | ——— |
| **Grand Total** | **4126** |

### Prices
July 2023 prices without shipping

#### Stage 1
| Item  | Price |
| :--- | ---: |
| Modem | 117 |
| Router | 495 | 
| Access Point | 124 |
| Switch | 144 | 
| Cabinet | 374 |
| Cabinet wheel set (estimate) | 40 |
| Cabinet fan upgrade | 64 |
| SFP+ thunderbolt adapter (Mac) | 197 |
| SFP+/RJ45 WAN Transceiver | 51 |
| 4 x SFP28 Transceiver | 120 |
| 6 x SFP+ Transceiver | 98 |
| Fibre network cables | 80 |
| 2 x Cat.8 50cm | 20 |
| WAN TAE cable | 9 |
| ———————————————— | ——— |
| **Total** | **1933** |

#### Stage 2
| Item  | Price |
| :--- | ---: |
| Fritz!Box rackmount | 110 |
| Windows Mini-PC (used) | 235 |
| UPS | 583 |
| USB cable | 7 |
| 1 x Cat.8 50cm | 10 |
| 1 x Cat.8 1m | 11 |
| ———————————————— | ——— |
| **Total** | **956** |

#### Stage 3
| Item  | Price |
| :--- | ---: |
| TinyPilot Voyager 2a | 463 |
| Dual SFP+ adapter (Mac) | 764 |
| 1 x Cat.8 50cm | 10 |
| ———————————————— | ——— |
| **Total** | **1237** |

## Networking hardware
### Modem
* ZyXEL VMG3006-D70A VDSL2 SuperVectoring Bridge Modem/Router
* https://www.zyxel.com/de/de/products/dsl-cpe/vdsl2-supervectoring-bridge-modem-vmg3006-d70a/specifications
* NOTE: bridge modem mode
* Price: 117

### Router
* MikroTik CCR2004-1G-12S+2XS
* https://mikrotik.com/product/ccr2004_1g_12s_2xs
* 2 x 25GbE SFP28, 12 x 10GbE SFP+, 2 x 1GbE RJ45 (1/0, 0/1, management)
* Price: 495

### Access point
* MikroTik hAP ax³
* https://mikrotik.com/product/hap_ax3
* WiFi 6, 1 x 2.5GbE, 4 x 1GbE
* Price: 124

### Switch
* ZyXEL XGS1210-12
* https://www.zyxel.com/us/en-us/products/switch/12-port-web-managed-multi-gigabit-switch-with-2-port-2-5g-and-2-port-10g-sfp-xgs1210-12/specifications
* managed, 2 x 10GbE SFP+ uplink, 2 x 2.5GbE, 8 x 1GbE
* Price: 144

## Cabinet hardware
### Server cabinet (silent rack)
* ZPAS SJB 19" RAL9005 (18U, 871cm height, Calvados)
* WZ-6729-01-04-161-BBL
* https://zpasgroup.de/schraenke-und-racks/4-sjb-19-netzwerkschrank.html
* https://www.ebay.de/itm/252410060506
* included: complete set without wheels
* Price: 374

#### Wheels
* ZPAS WZ-3987-20-00-000
* Price (estimate): 40

#### Fan upgrade
* 2 x Noctua NF-A12×25 LS-PWM (4-pin, 120x25cm, 12.1dB, LNA included)
* https://noctua.at/en/nf-a12x25-ls-pwm/specification
* Price: 64 (2 x 32)

### Fritz!Box rackmount
* https://www.ebay.de/itm/256104628861
* NOTE: Fritz!Box in IP Client Mode for VoIP & Fax + switch
* Price: 110

### Cables
#### Fibre
##### 2 x 20cm
* https://www.amazon.de/dp/B09C1ZVRL2/
* NOTE: router to switch (dual SFP+ patch)
* Price: 40 (2 x 20)

##### 2 x 50cm
* https://www.amazon.de/dp/B09C1ZVRL2/
* NOTE: router to server (dual SFP28 internal connection)
* Price: 28 (2 x 14)

##### 1 x 5m
* https://www.amazon.de/dp/B09C1ZVRL2/
* NOTE: router to Mac (single SFP+ external connection)
* Price: 12

#### RJ45
##### 1 x TAE VDSL 10m
* CoxBox: https://www.amazon.de/dp/B011J4XWLY/
* NOTE: WAN to modem (external connection)
* Price: 9

##### 4 x Cat.8 50 cm
* SnowKids: https://www.amazon.de/gp/product/B0BKZV81Y6/
* NOTE: Modem to Router, Fritz!Box to switch, MicroPC to switch, TinyPilot to switch (internal connections)
* Price: 40 (4 x 10)

##### 1 x Cat.8 1m
* SnowKids: https://www.amazon.de/gp/product/B0BKZV81Y6/
* NOTE: UPS to switch (internal connection)
* Price: 11

#### USB
* USB Type-B to USB Type-A cable (50cm or 1m)
* https://www.amazon.de/dp/B086ZHLW5T/
* NOTE: UPS to server (USB2.0)
* Price: 7

### Transceivers
#### WAN Transceiver
* Mikrotik S+RJ10
* https://mikrotik.com/product/s_rj10
* NOTE: auto-negotiating SFP+ to RJ45 transceiver
* Price: 51

#### 4 x SFP28 transceiver
* 10Gtek GP-25GSFP-1S
* https://www.amazon.de/dp/B0BVLWQ1Z6/
* NOTE: 2 x router, 2 x server
* Price: 120 (4 x 30)

#### 6 x SFP+ transceiver
* 10Gtek 
* https://www.amazon.de/dp/B013WFH7C8/
* NOTE: 3 x router, 1 x Mac, 2 x switch
* Price: 98 (64+34)

## Additional hardware
### Thunderbolt fibre ethernat adapter for Mac
* QNAP QNA-T310G1S
* https://www.qnap.com/en-us/product/qna-t310g1s/specs/hardware
* Price: 197

#### Alternative #1
* SonnetTech Twin10G SFP+
* https://www.sonnettech.com/product/twin10g-sfp-tb3/techspecs.html#techspecs
* Price: 764

#### Alternative #2
* SonnetTech Twin25G
* https://www.sonnettech.com/product/twin25g/techspecs.html#techspecs
* NOTE: needs 25GbE SFP28 switch
* Price: 1042

### Windows Mini-PC
* HP Elitedesk 800 G4 SFF (Windows 11 compatible)
* https://www.hardware-corner.net/desktop-models/HP-EliteDesk-800-G4-SFF/
* NOTE: for firmware flashing, Windows VMs & MikroTik management
* Price (used): 235

### KVM
* TinyPilot Voyager-2a
* https://tinypilotkvm.com/product/tinypilot-voyager2a
* Price: 463

### UPS
* APC Smart UPS SMX750I USV 750VA (incl. rackmount option), 600 W effective
* https://www.apc.com/shop/hr/en/products/APC-Smart-UPS-X-Line-Interactive-750VA-Rack-tower-convertible-2U-230V-8x-C13-IEC-SmartSlot-Extended-runtime/P-SMX750I
* NOTE: 15 minutes uptime
* Price: 583