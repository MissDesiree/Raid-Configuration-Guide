# Raid-Configuration-Guide

Overview
This project provides step-by-step instructions for configuring RAID 0 (Striped) and RAID 1 (Mirrored) on a system using the BIOS RAID Configuration Utility. The guide walks through enabling RAID mode in the BIOS, creating a RAID 0 array for performance, and a RAID 1 array for redundancy.
Prerequisites
Before starting, ensure you have:
A computer with a BIOS that supports RAID configuration.
At least two SATA drives.
Basic knowledge of navigating BIOS settings.
Steps to Configure RAID
1. Enable RAID Mode in BIOS
Power on the computer.
When the BIOS load screen appears, press Delete or F2 to enter the BIOS setup.
Navigate to System Configuration > SATA Operation.
Select RAID On and apply the changes.
Exit BIOS and restart the computer.
When prompted, press CTRL + I to enter the RAID Configuration Utility.
2. Create a RAID 0 (Striped) Array
In the RAID Configuration Utility, highlight Create RAID Volume and press Enter.
In the Name field, enter LD1.
Press TAB to highlight RAID Level, then use the arrow keys to select RAID0 (Stripe).
Press TAB to highlight Select Disks and press Enter.
Use the arrow keys to highlight ID 1 and press the Space bar to select the disk.
Use the arrow keys to highlight ID 2 and press the Space bar to select the disk.
Press Enter to confirm disk selection.
Press TAB to highlight Create Volume and press Enter.
Press Y to confirm and create the RAID 0 array.
3. Create a RAID 1 (Mirrored) Array
In the RAID Configuration Utility, highlight Create RAID Volume and press Enter.
In the Name field, enter LD2.
Press TAB to highlight RAID Level, then use the arrow keys to select RAID1 (Mirror).
Press TAB to highlight Select Disks and press Enter.
Use the arrow keys to highlight ID 1 and press the Space bar to select the disk.
Use the arrow keys to highlight ID 2 and press the Space bar to select the disk.
Press Enter to confirm disk selection.
Press TAB to highlight Create Volume and press Enter.
Press Y to confirm and create the RAID 1 array.
Verification
After setup, restart the computer and enter the BIOS to confirm the RAID arrays are detected.
Use system utilities to verify RAID status and performance.
Notes
RAID 0 provides performance benefits but lacks redundancy.
RAID 1 ensures data redundancy by mirroring disks.
Ensure important data is backed up before configuring RAID.

