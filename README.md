# assemblers-almanac
Fork of https://gitlab.com/qhaos/assemblers-almanac in github form

# Assemblers Almanac

This document describes the resources the regulars at the [Assemblers Community Discord sever](https://discord.gg/fxqBhgasTN) like to recommend. There are lots of different ways to learn, and everyone has their own preferences--so any number of references are given on each topic to supply diversity. And also depth.

There are resources here about learning assembly language on different platforms, but also many related subjects, since assembly language programmers generally like to learn things from the bottom up.

### [Discord](https://discord.gg/fxqBhgasTN) | [Matrix](https://matrix.to/#/+asm:fairydust.space)

## Table of Contents
- [8080, z80](#80)
- [x86](#x86)
- [ia64](#x86)
- [ARM](#arm)
- [Low-level Design](#lowlevel)
- [MIPS](#x86)
- [OSDev](#osdev)
- [Other](#other)
- [Windows Internals](#winternals)

<a name="80"></a>
## 8080/z80
- [XLT86 8080 to x86 translator](http://www.s100computers.com/Software%20Folder/Assembler%20Collection/Digital%20Research%20XLT86%20Manual.pdf)
<a name="x86"></a>
## x86
- [64-bit](https://chromium.googlesource.com/chromiumos/docs/+/master/constants/syscalls.md#x86_64-64_bit) and [32-bit Linux syscalls](https://chromium.googlesource.com/chromiumos/docs/+/master/constants/syscalls.md#x86-32_bit)
- [Fleix Cloutier's x86 and amd64 instruction reference](https://www.felixcloutier.com/x86/) Cloutier's venerable instruction set reference for the x86 processors is derived from the Intel manuals, but stripped to a very readable, hyperlinked online format.
- [flat assembler (FASM) programmer's manual](https://flatassembler.net/docs.php?article=manual) The Flat Assembler (FASM) is a multi-pass optimizing assembler for x86 architecture.
- [int table](https://stanislavs.org/helppc/int_table.html) The int table is a nice real-mode interrupt reference for Intel hardware, IBM PC BIOS and DOS interrupts.
- [Ralf Brown's Interrupt List](http://www.ctyme.com/rbrown.htm) The the 90s, Ralf Brown maintained a giant list of documentation for various interrupts and BIOS calls. That list has been converted to HTML and is searchable and hyperlinked, now.
- [Tiny Guide to x86 Assembly](https://cs.dartmouth.edu/~sergey/cs258/tiny-guide-to-x86-assembly.pdf)
- [*Low-Level Programming*](https://www.amazon.com/Low-Level-Programming-Assembly-Execution-Architecture/dp/1484224027/) Zhirkov's book describes computer architecture practically, using hands-on examples with the x64 arhictecture on Linux, using the `nasm` and `gcc` toolchains. 


## Itanium
<a name="ia64"></a>
- [New Old Thing - Itanium](https://devblogs.microsoft.com/oldnewthing/page/2?s=itanium)



## ARM
<a name="ARM"></a>
- [64-bit](https://chromium.googlesource.com/chromiumos/docs/+/master/constants/syscalls.md#arm64-64_bit) and [32-bit Linux syscalls](https://chromium.googlesource.com/chromiumos/docs/+/master/constants/syscalls.md#arm-32_bit_EABI)
- [*Computer Organization and Design* (ARM Edition)](https://www.amazon.com/Computer-Organization-Design-ARM-Architecture/dp/0128017333/) This edition of the Patterson and Hennessy books uses the ARM architecture for its teaching. The book investigates all aspects of the processor, including I/O, execution, instruction decoding, and cache memory strategies.
The book also includes detailed low-level design discussions--gate-level implementations of various subsystems, and work on VHDL descriptions for those subsystems. Attention is given to optimization techniques, along with the basics.

## Low-Level Design
<a name="lowlevel"></a>
- [*Hacker's Delight*](https://www.amazon.com/Hackers-Delight-2nd-Henry-Warren/dp/0321842685/) This book is a compendium of notes 
about low-level programming. Tricks about bit-twiddling, checking for overflow or underflow conditions, multi-word math operations, integer operations (like roots and lograithms), and so on ... are all presented with light
  mathematical rigor and clear pseudocode for implementation in whatever language you're targeting.

## OSDev
<a name="osdev"></a>
- [AMD64 Programming Manual - Vol2. Systems Programming](https://www.amd.com/system/files/TechDocs/24593.pdf)
- [*Operating Systems: Three Easy Pieces*](https://www.amazon.com/Operating-Systems-Three-Easy-Pieces/dp/198508659X/) This book treats operating systems in three "easy" pieces: virtualization, concurrency, and persistence. Also downloadable from [ostep.org](http://www.ostep.org/). The chapters are all only a dozen or so pages long, and easily digested. The diagrams could be better-drawn, and examples often don't build on each other and instead change context and assumptions from one to the next.
- [*Operating Systems Concepts*](https://www.amazon.com/gp/product/B07CVKH7BD/) by Abraham Silberschatz. Older versions of this book are great. Once regarded one of the best OS textbooks available, the newest 10th edition is hampered by the recent trend to offer goofy packaging for text books: online only, online-bundled codes, and loose-leaf bindings for three-ring binders. The treatment of scheduling and memory management are unparalleled.
- [*Modern Operating Systems*](https://www.amazon.com/Modern-Operating-Systems-Andrew-Tanenbaum/dp/013359162X) by Andrew Tanenbaum and Herbert Bos. The 4th edition of this book revises this seminal work for newer concurrency and caching models. Another top-tier textbook, the deep treatment of design and implementation tradeoffs is well-regarded.

<a name="other"></a>
## Other

<a name="winternals"></a>
## Windows Internals

- [*Windows Internals*, Part 1](https://www.amazon.com/Windows-Internals-Part-architecture-management/dp/0735684189/) and [Part 2](https://www.amazon.com/gp/product/B08F5HLRBD). Russinovich, one of Microsoft's Distingushed Engineers, along with his co-authors disucsses
every aspect of the design and implementation of Windows' internal systems. This book explains Windows' driver model, its memory management structure and algorithms, its message and event handling architectures, and everything else.
- [*Inside Windows Debugging*](https://www.amazon.com/Inside-Windows-Debugging-Debugging_p1-Developer-ebook/dp/B00JDMPHN6/) is a book about how to debug programs in Windows. It goes over the Windows debugging tools -- Visual Studio and WinDbg -- and the SDKs that install them.
It also covers the infrastructure in Windows for debugging and tracing. Further, it gives attention to post-mortem debugging with dump collection tools, and describes how to support widely-distributed applications which often fail mysteriously in the field.
  There are several chapters about debugging difficult scenarios and common troubleshooting techniques.