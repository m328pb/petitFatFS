# petitFatFS
Sub-set of FatFs module for tiny 8-bit microcontrollers

# Credits
All credits goes to Mr. Chang for his great work: https://elm-chan.org/fsw/ff/00index_p.html
Intentioon of this repo is to allow using the lib as platformio library. No changes are made and none are planed to orginal code.

# Use
For use see https://elm-chan.org/fsw/ff/00index_p.html.
Petit FatFs module is completely separated from disk I/O layer, it requires following functions to lower layer to read data from storage device. The low level disk I/O module is not a part of Petit FatFs module and it must be provided by user: 
disk_initialize - Initialize storage device
disk_readp - Read a partial sector
disk_writep - Divided write to a sector
For example of implementation see https://github.com/m328pb/sd for implementation on ATmega328

# Features
- Very Small RAM Consumption (44 Bytes Work Area + Certain Stack).
- Very Small Code Size (2K-4K bytes).
- FAT12, FAT16 and FAT32.
- Single Volume and Single File.
- Streaming File Read.
- File Write Function with Some Restrictions.
