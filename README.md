# 2taspian
2Taspian is a x86 Grub Platform used to process memory in the TASP2 Kernel.

# What does 2Taspian do?
2Taspian processes Memory Addresses & Offsets to load them into the EXFS Partition, which boots Taspin OS.

# Features
2Taspian Platform does the following:
* Memory Threading: 2taspian processes memory offsets and addresses to load them into the EXFS Partition, created by the Taspin OS.
* Offset Editing: 2Taspian allows you to edit offsets of the system to your liking.
* Process Executing: 2taspian is able to execute programs when a task is fired, on different times.
* Process Extension Acceleration (PEA): 2taspian extends memory and overwrites the following sections for it to be able to be executed: .RDATA, .TEXT
* Data Execution Prevention: 2taspian has an AES-256 restriction, that uses RKEYS to encrypt programs, for them to be checked by the kernel, then executed on the Internal Interface.

# Data Execution Hosts (DEH, PAP)
DEH uses the 2Taspian platform to execute memory with special flags and commands, which are:
* JLC: Jump if Local = Jumps to an address if LOCAL is running. (LOCAL = ShellHost)
* ADM: Add Memory = Add a memory offset to a block of memory.
* SUM: Subtract Memory = Remove a memory offset from a block of memory.
* ITC: Execute Internal Terminal Constant = Execute a constant command in the ITC Processor (x32), for it to be fired to the Internal Interface (I.I.)
* ADP: Add Process = Add a process to the Internal Interface (I.I)
* SUP: Remove Process = Remove a process from the Internal Interface (I.I)
* DCL: Execute Data Constant Library = Execute a Data Constant from a Data Constant Library (DCL)

# Identification
2Taspian can be identified with its platform, with the following:
* SHA Hash: 6401141935546a920e982199a9584414da299764 = Identifies TASP Partition Type.
* MD5 Hash: fec376d901538e742b921161497a5193 = Identifies GRUB Version and CodeName.
* DAPL Address: 0x4311FF1135FF6 = Identifies Platform Type = Current Type: 1TS (x32)
* A-DAPL Address: 0x5311FF561234FF19FF0 = Identifies Platform Type = Current Type: 2TS (x64)
* B-DAPL Addres: 0xFF11FF3311FF44 = Identifies Platform Type = Current Type: TSD (Default, x86)


# Apply 2Taspian to your SYSTEM
2Taspian is appliable to the following: UEFI, EFI
2Taspian is also available on the following Linux Roots: Ubuntu, Debian, Pop!_OS

To apply 2Taspian to your system, do the following steps:
* Step 1: Load /bootmanager/winpeg-pe.deb into /EFIFILESYSTEM/EFI or /EFIFILESYSTEM/DVD.
* Step 2: Add /libraries/apidve.app to [BOOT-PARTITION]:\Windows\Boot
* Step 3: Allow 2taspian to load by loading /ldr2/2taspldr into [BOOT-PARTITION]:\Windows\Setup\Scripts
* Step 4: Reboot into BIOS Screen / Menu and boot from "ADD: 2Taspian LDR 16GB"
