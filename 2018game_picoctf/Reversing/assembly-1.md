
# assembly-1

## Q

What does asm1(0x255) return? Submit the flag as a hexadecimal value (starting with '0x'). NOTE: Your submission for this question will NOT be in the normal flag format. Source located in the directory at /problems/assembly-1_1_3d18f926da00c5acd1dbe672938d342d.

## S

asm1(0x255)

.intel_syntax noprefix
.bits 32

.global asm1

asm1:
    push    ebp
    mov ebp,esp
    cmp DWORD PTR [ebp+0x8],0xea // 0x255 > 0xea ,jmp part_a
    jg  part_a
    cmp DWORD PTR [ebp+0x8],0x8
    jne part_b
    mov eax,DWORD PTR [ebp+0x8]
    add eax,0x3
    jmp part_d
part_a:
    cmp DWORD PTR [ebp+0x8],0x6 // 0x255 > 0x6 , jmp part_c
    jne part_c
    mov eax,DWORD PTR [ebp+0x8]
    sub eax,0x3
    jmp part_d
part_b:
    mov eax,DWORD PTR [ebp+0x8]
    sub eax,0x3
    jmp part_d
    cmp DWORD PTR [ebp+0x8],0x126
    jne part_c
    mov eax,DWORD PTR [ebp+0x8]
    sub eax,0x3
    jmp part_d
part_c:
    mov eax,DWORD PTR [ebp+0x8] // eax == 0x255
    add eax,0x3                 // eax += 0x3 , eax == 0x258
part_d:                         // ret eax
    pop ebp
    ret

## A

0x258


