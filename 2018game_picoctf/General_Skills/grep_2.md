
# grep 2

## Q

This one is a little bit harder. Can you find the flag in /problems/grep-2_1_ef31faa711ad74321a7467978cb0ef3a/files on the shell server? Remember, grep is your friend.

## S

grep -e 'CTF{.*}' -R *
    files4/file20:picoCTF{grep_r_and_you_will_find_4baaece4}

## A

picoCTF{grep_r_and_you_will_find_4baaece4}


