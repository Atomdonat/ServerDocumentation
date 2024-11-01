# Rack
![[Rack_Layout.drawio.png]]

## Rack
- **Manufacturer:** StarTech
- **Product Name:** 4POSTRACK12U

![[Serverschrank_Diagram.pdf]]

## Management and Backupserver

## DMZ Router
- **Manufacturer:** Dell
- **Product Name:** [OptiPlex 7010 MT](https://www.hardware-corner.net/desktop-models/Dell-OptiPlex-7010-MT/) (Service-Tag: 55V36Y1; 2012)
- **CPU:** 3rd Gen Intel Core i3-3220 Processor (Dual Core, 3.30GHz, 3MB, w/ HD2500 Graphics)
- **Mainboard:** E93839 LA0531
- **RAM:** 4 DIMM DDR3-1333/1600 max 32 GB
- **GPU:** integrated
- **Storage:**
	- 4x SATA
- **PCI Slots:** PCIe 3.0 x16; PCIe 2.0 x1; PCI; PCIe 2.0 x16 (wired x4)
- **Drive bays:** (2x) 3.5in/2.5in; (2x) 5.25in
- **Power:** ATX 275 W
- **Network:** Gigabit Ethernet (10/100/1000 Mbps)
- **Modifications:**

## Router
- **Manufacturer:** AVM
- **Product Name:** Fritz!Box 4040
- **Architecture:** ARMv7 Processor rev 5 (v7l)
- **Firmware:** OpenWrt 22.03.5
- **MGMT:** LuCI openwrt-22.03
- **Network:**
	- 1xWAN (RJ-45, 1Gbit/s)
	- 4xLAN (RJ-45, 1Gbit/s)
- **Power:** (18W, barrel tip 5.5mm/2.5mm)

## Switch
- **Manufacturer:**
- **Product Name:**
- **CPU:**
- **RAM:**
- **Network:**
- **Features:**
- **Power:** 

## TrueNAS Server
- **Manufacturer:** Dell
- **Product Name:** PowerEdge R520
- **CPU:** 2x Intel Xeon E5-2407 (2.2GHz, 10MB Cache)
- **RAM:** 4x Hynix HMT325R7CFR8A (DDR3, 2GB, 1333MHz, 1.35V)
- **GPU:** ---
- **Storage:**
	- 1x Intenso High Performance 3813430 (SATA3 6Gb/s, 2.5", 120GB, 520MB Cache)
	- 2x Seagate Cheetah ST3300657SS (SAS 6Gb/s, 3.5", 300GB, 15K.7, 16MB Cache)
	- 2x Seagate Savvio ST300MM0006 (SAS 6Gb/s, 2.5", 300GB, 10K.6, 64MB Cache)
	- 4x Seagate Savvio ST600MM0006 (SAS 6Gb/s, 2.5", 600GB, 10K.6, 64MB Cache)
- **Power:** 2x Dell SPS 0N24MJ (495W, 80+ Platinum, Redundant, C13)
- **Network:** 2x Broadcom BCM5720 (RJ-45, 1Gbit/s)
- **MGMT:** iDRACv7 (RJ-45)
- **Modifications:** DeLOCK Slim SATA (5.25" to 2.5"; no mounting holes for og-hotswap-safety)

## AMP Server
- **Manufacturer:** Dell
- **Product Name:** PowerEdge R520
- **CPU:** 2x Intel Xeon E5-2407 (2.2GHz, 10MB Cache)
- **RAM:** 8x Micron MT18KSF51272PDZ-1G4M1FF (DDR3, 4GB, 1333MHz, 1.35V)
- **GPU:** ---
- **Storage:**
	- 1x Intenso High Performance 3813430 (SATA3 6Gb/s, 2.5", 120GB, 520MB Cache)
	- 3x Seagate Constellation ES ST2000NM0001 (SAS 6Gb/s, 3.5", 2TB, 7.2K, 64MB Cache)
- **Power:** 2x Dell SPS 0N24MJ (495W, 80+ Platinum, Redundant, C13)
- **Network:** 2x Broadcom BCM5720 (RJ-45, 1Gbit/s)
- **MGMT:** iDRAC7 (RJ-45)
- **Modifications:** DeLOCK Slim SATA (5.25" to 2.5"; no mounting holes for og-hotswap-safety)

# Cable Management

![[Cable_Management.pdf]]

[Patch Cable Color Code and Standards](https://www.cablewholesale.com/blog/index.php/2022/01/26/different-cable-colors-and-their-uses-the-complete-guide/):

- Grey: standard network connections
- Black: used as a generic, default color
- Purple: non ethernet digital connections
- Blue: terminal server connections
- Green: crossover connection (direct connection; no Switch involved)
- Yellow: POE connection
- Orange: non ethernet, analog connections
- Pink: additional color option for any function
- Red: IP cameras
- White: additional color option for any