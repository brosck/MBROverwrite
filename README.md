<h1 align="center">「💽」MBR Overwrite malware for linux</h1>

<p align="center"><img src="/assets/message.png"></p>

<p align="center">The MBR virus has the function of staying in the Master Boot Record (MBR) causing the system to load the sector infected by the virus after being initialized. This type of virus causes an infection in the Basic Input/Output System (BIOS) using Disk Operating System (DOS) commands to infect the disk.</p>


This repository was created with the intention of demonstrating the attack of this virus from the execution of it in a Linux system.

**Note**: **DO NOT RUN** on your personal machine, use a virtual machine to do the experiment.

## Demonstration:

<p align="center"><img src="/assets/demo.gif"></p>

## Requirements:

* GCC
* NASM

## Build:

In the file ```mbroverwrite.c``` in ```#define DISK "/dev/sda"``` is indicating the disk where will be replaced by the payload.

In the file ```mbroverwrite.c``` in ```unsigned char payload[]``` is storing the compiled file ```message.asm```, where the values are in HEX.

```
$ git clone https://github.com/Brosck/MBROverwrite.git
$ cd MBROverwrite
$ make
$ sudo ./mbroverwrite
```

## Buy me a coffee?

<img src="https://static.livepix.gg/images/logo.svg" height="50" widght="50">

[LivePix](https://livepix.gg/mrempy)

<img src="https://play-lh.googleusercontent.com/aMb_Qiolzkq8OxtQZ3Af2j8Zsp-ZZcNetR9O4xSjxH94gMA5c5gpRVbpg-3f_0L7vlo" height="50" widght="50">

[Buy me a coffe](https://www.buymeacoffee.com/mrempy)
