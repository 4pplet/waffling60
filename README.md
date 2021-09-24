# waffling60

waffling60 is a multilayout 60% PCB with support for common ANSI and ISO layouts and split space. The PCB is split into different versions:
- One ALPS version with different assembly options.
- One MX version with different assembly options.
- One dedicated version of the MX PCB to fit bakeneko/unikorn cases.
- One dedicated version of the MX PCB made to fit ai03 Polaris.
- Current multi-layout Hot swap version is depricated and not indended for update

## Features:
- QMK & VIA
- USB-C
- ATmega32U2 in QFN and QFP
- RGB-led under/close to capslock for MX-versions
- Cherry PCB-stab support
- Split space
- ISO and ANSI
- USB horizontal placement is classic GH60, same as GH60, plain60, voyager60 etc for the normal MX and ALPS-version
- SE-version is adapted for Polaris (stab-rotations, outline and USB-placement), make sure to order 1.2 mm thickness when manufacturing these. 
- On solder versions: Switch rotation is only with LED facing south. **On hot swap version:** Switch rotation is North, south and 90 degree, MAKE SURE TO CHECK SO THIS WILL NOT CAUSE KEYCAP ISSUES FOR YOU. Clip-in stabilziers is recommended for ISO-enter stab for hot-swap version

## **Disclaimer/note:**
- **Important:** SE version of waffling60 (Polaris compatible version) are not officially endorsed by ai03 and ai03 takes no responsibility or offers any support for these if there is any issue. I have been given permission to open source and offer these for sale.**

## Layout support MX: 
![alt text](./readme-images/layout_support.jpg "Layout support")

## MX Solder, multiple assembly options
![alt text](./readme-images/waffling60-MX_Rev_B4_Tray.jpg "PCB View - Rev A")

## ALPS Solder, multiple assembly options
![alt text](./readme-images/waffling60-ALPS_Rev_B5_Tray.jpg "PCB View - Rev A")

## SE ("Bolaris")
![alt text](./readme-images/waffling60-SE_Rev_B2.jpg "PCB View - Rev A")

## BK ("Bakeneko")
![alt text](./readme-images/waffling60-BK_Rev_B4.jpg "PCB View - Rev A")

## Instructions for manufacturing.

The Project can be assembled in three different configurations:
1. Traditional tray mount with USB-C connector
2. Daughter board connector in two different configurations:
	- Bakeneko position
	- Position for cases made for wilba PCB's
In most versions, a "all" configuration is also included, this is not a "one config fits all", it's intended to be used for making your own config.

## For ordering:
The following files are needed for the PCB Fab:
- BOM (contains component specifications)
- Pick and Place (contains component placement data)
- Gerber (contains PCB drawings and drill files)
- (optional) Assembly drawing, for manual assembly

Select the files for the desired configuration. Gerber and Pick and Place files will be the same for all three configurations, BUT!, you need to select the correct BOM for your configuration.

If you want to make a bakeneko compatible PCB, select the bakeneko BOM when ordering PCB's.

## Releases
Files for manufacturing can be found in releases.

Releases are split into the following versions of the PCB: (note: not the same as configuration)
- Waffling60 MX, a MX solder PCB in three configurations: Bakeneko, Tray and Wilba
- Waffling60 Alps, a ALPS solder PCB in three configurations: Bakeneko, Tray and Wilba
- Waffling60 SE, a PCB compatible with AI03 Polaris, same layout support as the regular MX PCB. Order in 1.2mm thickness for use with the Polaris. Same flexcut and stab rotations as the OG PCB.
- Waffling60 BK, a dedicated bakeneko version of the regular MX PCB.
- Waffling60 MXHS, a depricated hotswap PCB using the same layout support as the solder PCB. Note that the revision is still B2, stab rotations have been changed on the solder PCB's.

## FR4 Plates:
- Tray mount plate: Stab rotations have been changed from revision B2 to B3, so version V1 and V2 of the plate is no longer compatible with the newest revisions.
- Polaris plate: Compatible with OG polaris PCB and waffling60SE

## For clarity
- Revision: When updating the PCB I bump the revision. The revision is specified with a letter and a number. For big changes, the letter is changed (usually also include code changes), for minor changes, only the number is bumped.
- Version: Version specifies different switch types, PCB's specific to certain cases etc.
- Configuration: Different assembly options for a specific version of waffling60 

## Revision history:
- Rev A1: Initial prototype based on Steezy60 Alps-version.
- Rev A2: Rotate Fn-switch (split RShift) on solder version. Rotate LShift stabilizer on both versions. To rotate left shift stabilizer on hot-swap pcb, adjacent sockets is also rotated.
- Rev B1: Changed matrix and diode under capslock for cleaner routing and easier software implementation in QMK for LED
- Rev B2: Moved daughter board connector to allign all projects with a similar horisontal position and a identical vertical position. Removed flex-cuts for more preictable feel in "traditional" cases.
- Rev B3: Changed stab rotation to what's more common today. Alligns with most common projects and cases. Updated PCB outline. Moved daughter board connector for better position in bakeneko. Added flexcuts again, but a simpler one.
- Rev B4: Changes to PCB outline, added support for bakeneko V3 and possibly KEI
- Rev B5 - Alps: Adding symetrical split space support using AEK-keycaps and adding RGB led below capslock switch for use with transparent switches (matias)

