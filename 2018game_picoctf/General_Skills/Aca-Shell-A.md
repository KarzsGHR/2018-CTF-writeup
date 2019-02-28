
# Aca-Shell-A

## Q

It's never a bad idea to brush up on those linux skills or even learn some new ones before you set off on this adventure! Connect with nc 2018shell.picoctf.com 58422.

## S

nc 2018shell.picoctf.com 58422
```
Sweet! We have gotten access into the system but we aren't root.
It's some sort of restricted shell! I can't see what you are typing
but I can see your output. I'll be here to help you along.
If you need help, type "echo 'Help Me!'" and I'll see what I can do
There is not much time left!
```
~/$ ls
```
blackmail
executables
passwords
photos
secret
```
~/$ cd secret
```
Now we are cookin'! Take a look around there and tell me what you find!
```
~/secret$ ls -l
```
-rw-r--r-- 1 aca-shell-a_0 aca-shell-a_0  86 Jul  1  2018 intel_1
-rw-r--r-- 1 aca-shell-a_0 aca-shell-a_0 100 Jul  1  2018 intel_2
-rw-r--r-- 1 aca-shell-a_0 aca-shell-a_0  95 Jul  1  2018 intel_3
-rw-r--r-- 1 aca-shell-a_0 aca-shell-a_0  40 Jul  1  2018 intel_4
-rw-r--r-- 1 aca-shell-a_0 aca-shell-a_0  85 Jul  1  2018 intel_5
-rw-r--r-- 1 aca-shell-a_0 aca-shell-a_0  44 Jul  1  2018 profile_ahqueith5aekongieP4ahzugi
-rw-r--r-- 1 aca-shell-a_0 aca-shell-a_0  44 Jul  1  2018 profile_ahShaighaxahMooshuP1johgo
-rw-r--r-- 1 aca-shell-a_0 aca-shell-a_0  90 Jul  1  2018 profile_aik4hah9ilie9foru0Phoaph0
-rw-r--r-- 1 aca-shell-a_0 aca-shell-a_0  95 Jul  1  2018 profile_AipieG5Ua9aewei5ieSoh7aph
-rw-r--r-- 1 aca-shell-a_0 aca-shell-a_0  30 Jul  1  2018 profile_bah9Ech9oa4xaicohphahfaiG
-rw-r--r-- 1 aca-shell-a_0 aca-shell-a_0  34 Jul  1  2018 profile_ie7sheiP7su2At2ahw6iRikoe
-rw-r--r-- 1 aca-shell-a_0 aca-shell-a_0  75 Jul  1  2018 profile_of0Nee4laith8odaeLachoonu
-rw-r--r-- 1 aca-shell-a_0 aca-shell-a_0  34 Jul  1  2018 profile_poh9eij4Choophaweiwev6eev
-rw-r--r-- 1 aca-shell-a_0 aca-shell-a_0  89 Jul  1  2018 profile_poo3ipohGohThi9Cohverai7e
-rw-r--r-- 1 aca-shell-a_0 aca-shell-a_0  50 Jul  1  2018 profile_Xei2uu5suwangohceedaifohs
Sabatoge them! Get rid of all their intel files!
```
~/secret$ rm intel_*
```
Nice! Once they are all gone, I think I can drop you a file of an exploit!
Just type "echo 'Drop it in!' " and we can give it a whirl!
```
~/secret$ echo 'Drop it in!'
```
Drop it in!
I placed a file in the executables folder as it looks like the only place we can execute frcom!d
Run the script I wrote to have a little more impact on the system!
```

~/secret$ cd ..
~/$ ls
```
blackmail
executables
passwords
photos
secret
```
~/$ cd executables
~/executables$ ls -l
```
-rwxr-xr-x 1 aca-shell-a_0 aca-shell-a_0 611 Jul  1  2018 dontLookHere
```
~/executables$ ./dontLookHere
```
 30d2 7095 92ca 47d4 76f0 117e 58f3 7b39 b950 09ff 9c68 2ca7 97b9 5c10 3cf1 b561 54e6 0984 2104 5e36 a889 3756 d7f6 29c7 c4d5
 5ddc fd08 bdcd 44f1 9995 703d 3174 dc5a fabc f3f8 50d6 101e 49a4 a13a 6b98 119b cde6 5638 8336 a603 6977 d6e8 68ab b72c 7a92
 9a75 2c0c 7c26 7613 9e07 ac25 d22c 9704 da11 6d26 22d6 fe35 e051 416e 3e9d 711d 05ac ee3c d0a3 704a 9e56 7861 de95 3ac6 3965
 403f d2cf 620b 9d7f b8e3 1ace f1b2 43ab 3c10 116a f697 be0b e8af add2 82c6 3981 f5b1 e2e2 80ee 2aaa 326b d3fd 640e 779d 0f6c
 1223 020a 8a03 15ff b663 90d3 23ef f7e3 25c0 ba19 e74c 494d 3d28 93e0 8c86 dc38 b484 3850 1f14 152f 38ab a5ed 0e17 7719 82b3
 dabe 7631 397f d257 e76c 67ed a134 ef14 1681 ed82 ce8c cf89 d7c4 e3a9 31a9 04d0 edc4 7416 1701 fc79 cfae 2e7e f726 f70b 10b9
 78b1 c3d6 ba64 18cf f80b ef4b 88f9 8267 da1a f37a 2f30 9b94 b3c6 c97e a6c7 84d6 d4a2 cdb3 94e4 6443 c16b 42ed 21de 79ad 8add
 3913 d01d c880 61b7 08db dcb0 bdd4 1d9a 56a0 2160 5785 d370 d9ac 0496 7686 e11e c4d1 cee1 a5b0 5dc9 b71f 5d4e f5b4 2146 b89e
 7db7 765d e0b7 40f8 ee66 f40a 31ec fc2d 0e89 9f97 e610 559c 6c2b 9983 57a0 3995 257d 1b90 0631 7a37 3644 6d98 6ffe 4510 70b7
 bbcc 3545 b04b 5637 12cf efa3 83ec 7d35 d0d3 5003 d4b1 7e65 d1f3 7493 c3da 84e2 2fcb dd76 1903 1f99 12e4 c845 4b7a df40 a86f
 e6f6 9b98 46f7 34d2 e1fd 4946 f48e 7d60 da59 d037 6120 62fc a362 a378 95ae 5f38 2aec 5845 b12a 4b93 73b3 4f59 e9f6 9151 5ca5
 9523 7078 9163 d5fe 6bba 2013 1e79 f80a 80e1 7542 cd13 7f10 8345 b8b0 1f66 84ff 44b4 d02b 84b2 3dbe 0f8b 8de5 51a4 4224 9ebf
 4e97 512e fe2a 0eb4 1473 7d98 9049 25d6 80da 1aef 5380 6641 a44d f7d7 a4b3 829f 6d97 7fb0 9b98 7a15 2900 beb4 bfca b162 2c30
 4994 96a5 d438 a879 d374 02d2 30e2 9610 a4ec 5bd4 f6c8 db32 e6db f8cf d7f7 8db2 4e8f 4325 22c3 3f34 03c1 699f c718 362a 6ef0
 07f2 8937 80a3 c31f 33ef cf8c 6d26 a8c8 0fe7 fd52 ec2b 6fe1 2ea8 82e2 4857 7b42 16a7 d496 1a59 1504 7038 bb1d 1682 6ddc 4a63
 d7a7 b33c 0f02 a5eb 907c b0d1 9cb5 5eef d133 989e 5157 0800 e050 0ca9 a029 631c 1413 23c3 1250 af2c 45ef f5ce c2fc aa55 19b8
 4566 a315 1e69 51c5 2bdd 58fc d874 13b9 e7d3 c59d 0b52 859d 5bfe 7581 1aa0 7c81 2172 c66b 3e55 326d c1be ce17 6e83 ee78 af7f
 336e c701 0781 36a3 bb42 fe17 f02a 9431 4d93 af87 5ecc 32fa bd2f 49e7 6ce8 f5e3 4172 85dd 88ef 52af 72df b0f5 d4c6 847a 89c4
 669c 7bcd 6a08 91b1 3a76 430c 0817 74b6 5084 fd23 57ac 8c98 f595 b1d6 c6fd 60a6 56de b18d 21fc 169e e4e9 0a73 f8cc faa7 0503
 a63a 12e4 0c77 a23d fc6c 6499 116c 125c dd5c 94c2 a99a a842 01d6 9232 6da3 8764 6f6e e2b8 1dac 446b 1702 0a60 1171 3b90 f45d
 1c5f d160 5fac a346 3c63 f3d9 20b9 47f8 4fba 4e12 585c 781c 4ae0 ceb7 6192 0237 1605 7170 cbdf 75aa 2319 8151 d55e 6475 35a8
 e2fe af4e 035c bc39 1e77 243f b5dd a1c8 dc1e b745 5928 ffaa 4740 ce85 5309 4967 2d1c 6757 31c0 6a3e ab92 3c07 bcc0 d449 31f0
 a2a3 8138 5107 b047 fec0 d275 e9ec 255e 0175 c820 d08e 057e 2a3d 8d9d 561d 500b c7d3 bbf5 7bcd f22f 972c eb94 d729 5753 99f6
 af71 4ef5 dfe4 db8b 68fe 3845 9d7e 2350 371b 0a51 ccb4 48d4 b34f d3e2 5ba8 8039 30c6 b81d c293 2030 7765 5155 2221 f66f f710
 e76d 8df3 06f2 669c 51a7 21ce fde3 3482 ca7d 8301 df87 a4e2 fe2e 054c 7e34 e7c9 08ef 79de 4c72 5cac c58c 32fc 666f 7536 f013
 7d7f 56c3 2526 d9bd 3cac 098f fa46 d5f2 418c bc20 41c5 850b cf31 9e29 8c7c ad82 6eb1 e622 07a0 d907 ce3b 4f8f 9b29 0092 ec3c
 5167 17cd f7ce 0c88 1319 f211 30e0 c610 0723 d9c0 af27 9311 b6e9 054a 3ee9 f12a 7609 8059 ae2a 7737 8095 4a3a 6dfb a967 1181
 2b69 ef54 96af 9c09 b5f2 4fed dd3e aba0 cb73 7b0a cf5a 50cc f206 3c01 768a ba30 347e 0a61 c01f f9b7 21ab 61c7 97f9 3d10 d749
 4ab2 fe0b d95f 40cf e56d 6cb6 ed05 d95f f887 ef42 01ea b70f 0b70 d724 8bc5 ee34 2561 1d69 4816 e8d2 a580 8ce1 072c c36b 77a1
Looking through the text above, I think I have found the password. I am just having trouble with a username.
Oh drats! They are onto us! We could get kicked out soon!
Quick! Print the username to the screen so we can close are backdoor and log into the account directly!
You have to find another way other than echo!
```
~/executables$ whoami
```
l33th4x0r
Perfect! One second!
Okay, I think I have got what we are looking for. I just need to to copy the file to a place we can read.
Try copying the file called TopSecret in tmp directory into the passwords folder.
```
~/executables$ cd ..
~/$ cp /tmp/TopSecret passwords
```
Server shutdown in 10 seconds...
Quick! go read the file before we lose our connection!
```
~/$ cd passwords
~/passwords$ cat TopSecret
```
Major General John M. Schofield's graduation address to the graduating class of 1879 at West Point is as follows: The discipline which makes the soldiers of a free country reliable in battle is not to be gained by harsh or tyrannical treatment.On the contrary, such treatment is far more likely to destroy than to make an army.It is possible to impart instruction and give commands in such a manner and such a tone of voice as to inspire in the soldier no feeling butan intense desire to obey, while the opposite manner and tone of voice cannot fail to excite strong resentment and a desire to disobey.The one mode or other of dealing with subordinates springs from a corresponding spirit in the breast of the commander.He who feels the respect which is due to others, cannot fail to inspire in them respect for himself, while he who feels,and hence manifests disrespect towards others, especially his subordinates, cannot fail to inspire hatred against himself.
picoCTF{CrUsHeD_It_4e355279}
```

## A

picoCTF{CrUsHeD_It_4e355279}
