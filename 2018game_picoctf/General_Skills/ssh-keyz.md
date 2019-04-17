
# ssh-keyz

## Q

As nice as it is to use our webshell, sometimes its helpful to connect directly to our machine. To do so, please add your own public key to ~/.ssh/authorized_keys, using the webshell. The flag is in the ssh banner which will be displayed when you login remotely with ssh to with your username.


## S

1.Crate sshras in local

2.cp rsa.pub to remote ~/.ssh/authorized_keys

3.ssh ...@pico... in local

https://kb.iu.edu/d/aews

## A

picoCTF{who_n33ds_p4ssw0rds_38dj21}


