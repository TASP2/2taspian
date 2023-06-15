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
