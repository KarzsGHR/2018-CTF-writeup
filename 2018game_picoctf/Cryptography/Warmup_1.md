
# Warmup_1

## Q

Crpyto can often be done by hand, here's a message you got from a friend, llkjmlmpadkkc with the key of thisisalilkey. Can you use this table to solve it?.
https://2018shell.picoctf.com/static/43f28853477d7b2ed52e0efbfb04dff7/table.txt

## S

ord() and chr() to build the function for the table

python3 -c "print(''.join([x for x in map(lambda x,y : chr((ord(x)-ord(y))%26+ord('A')),'llkjmlmpadkkc','thisisalilkey')]))"

## A

picoCTF{SECRETMESSAGE}


