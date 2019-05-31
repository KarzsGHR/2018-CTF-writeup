
# what base is this?

## Q

To be successful on your mission, you must be able read data represented in different ways, such as hexadecimal or binary. Can you get the flag from this program to prove you are ready? Connect with nc 2018shell.picoctf.com 31711.

## S

nc 2018shell.picoctf.com 31711


binary number to string

```
python -c 'b="01100011 01100001 01101011 01100101";print("".join([chr(int(x,2)) for x in b.split()]))'
```

hex number to string
```
python -c 'h="74657374";print("".join([chr(int(x+y,16)) for x,y in zip(h[::2],h[1::2])]))'
```


oct number to string
```
python -c 'c="143 157 155 160 165 164 145 162";print("".join([chr(int(x,8)) for x in c.split()]))'
```


## A

picoCTF{delusions_about_finding_values_68051dea}
