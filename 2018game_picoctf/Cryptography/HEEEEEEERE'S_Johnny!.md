
# HEEEEEEERE'S Johnny!

## Q

Okay, so we found some important looking files on a linux computer. Maybe they can be used to get a password to the process. Connect with nc 2018shell.picoctf.com 40157. Files can be found here: passwd shadow.
https://2018shell.picoctf.com/static/7a017af70c0b86ab002896616376499e/passwd
https://2018shell.picoctf.com/static/7a017af70c0b86ab002896616376499e/shadow


## S

unshadow passwd shadow > orpasswd
cat orpasswd
john orpasswd
```
Warning: detected hash type "sha512crypt", but the string is also recognized as "crypt"
Use the "--format=crypt" option to force loading these as that type instead
Using default input encoding: UTF-8
Loaded 1 password hash (sha512crypt, crypt(3) $6$ [SHA512 128/128 AVX 2x])
Press 'q' or Ctrl-C to abort, almost any other key for status
kissme           (root)
1g 0:00:00:03 DONE 2/3 (2019-02-28 19:31) 0.3164g/s 766.7p/s 766.7c/s 766.7C/s keller..mermaid
Use the "--show" option to display all of the cracked passwords reliably
Session completed

```

nc 2018shell.picoctf.com 40157
Username: root
Password: kissme
picoCTF{J0hn_1$_R1pp3d_1b25af80}


## A

picoCTF{J0hn_1$_R1pp3d_1b25af80}


