
# Recovering From the Snap

## Q

There used to be a bunch of animals here, what did Dr. Xernon do to them?
https://2018shell.picoctf.com/static/040c56434beb57348cc5032272c04350/animals.dd

## S

Mount and use 'strings' check
```
strings /Volumes/Transcend/2018pico/animals.dd | more

mkfs.fat
NO NAME    FAT16
This is not a bootable disk.  Please insert a bootable floppy and
press any key to try again ...
DACHSH~1JPG
OX     JPG
FROG    JPG
IRAFFE JPG
MUSIC   JPG
ABBIT2 JPG
RABBIT  JPG
HEFLAG JPG
JFIF
Exif
NIKON CORPORATION
NIKON D5100
2016:07:15 15:40:54
```
there are file losted.
use foremost to recover.

root@kali:/mnt/hgfs/Transcend/2018pico# foremost -t jpg -i animals.dd
```
Processing: animals.dd
|*|
```
root@kali:/mnt/hgfs/Transcend/2018pico# cd output/
root@kali:/mnt/hgfs/Transcend/2018pico/output# cat audit.txt
```
Foremost version 1.5.7 by Jesse Kornblum, Kris Kendall, and Nick Mikus
Audit File

Foremost started at Thu Feb 28 22:03:25 2019
Invocation: foremost -t jpg -i animals.dd
Output directory: /mnt/hgfs/Transcend/2018pico/output
Configuration file: /etc/foremost.conf
------------------------------------------------------------------
File: animals.dd
Start: Thu Feb 28 22:03:25 2019
Length: 10 MB (10485760 bytes)

Num  Name (bs=512)         Size  File Offset     Comment

0:  00000077.jpg         617 KB           39424
1:  00002277.jpg         380 KB         1165824
2:  00003041.jpg         248 KB         1556992
3:  00003541.jpg         314 KB         1812992
4:  00004173.jpg         458 KB         2136576
5:  00005093.jpg         383 KB         2607616
6:  00005861.jpg          39 KB         3000832
Finish: Thu Feb 28 22:03:25 2019

7 FILES EXTRACTED

jpg:= 7
------------------------------------------------------------------
```

One of them is flag.


## A

picoCTF{th3_5n4p_happ3n3d}


