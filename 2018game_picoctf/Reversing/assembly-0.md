
# assembly-0

## Q

What does asm0(0x2a,0x4f) return? Submit the flag as a hexadecimal value (starting with '0x'). NOTE: Your submission for this question will NOT be in the normal flag format. Source located in the directory at /problems/assembly-0_3_b7d6c21be1cefd3e53335a66e7815307.

## S

.intel_syntax noprefix
.bits 32

.global asm0

asm0:
    push    ebp
    mov ebp,esp
    mov eax,DWORD PTR [ebp+0x8] ;0x2a
    mov ebx,DWORD PTR [ebp+0xc] ;0x4f
    mov eax,ebx ; eax=ebx(0x4f)
    mov esp,ebp
    pop ebp
    ret


asm0(0x2a,0x4f)

Return EAX

## A

0x4f


