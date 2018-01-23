# rust-raspi-kernel

A Raspberry Pi Model B+ kernel written in Rust

## WARNING

Most of this is not guaranteed to work in a week.
Initial work based on https://medium.com/@thiagopnts/raspberry-pi-bare-metal-programming-with-rust-a6f145e84024.

Assumes running on a Raspberry Pi Model B+ (rev 1.2)

## How to build

`./build` will invoke all of the right commands. The resulting `kernel.tar` file contains everything needed to boot the kernel on the Raspberry Pi.

### Program versions

```shell
rustc --version
rustc 1.25.0-nightly (5965b7901 2018-01-19)
```

```shell
arm-none-eabi-gcc --version
arm-none-eabi-gcc (GNU Tools for Arm Embedded Processors 7-2017-q4-major) 7.2.1 20170904 (release) [ARM/embedded-7-branch revision 255204]
Copyright (C) 2017 Free Software Foundation, Inc.
This is free software; see the source for copying conditions.  There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
```

```shell
arm-none-eabi-objcopy --version
GNU objcopy (GNU Tools for Arm Embedded Processors 7-2017-q4-major) 2.29.51.20171128Copyright (C) 2017 Free Software Foundation, Inc.This program is free software; you may redistribute it under the terms ofthe GNU General Public License version 3 or (at your option) any later version.
This program has absolutely no warranty.
```

## Goals

### Immediate

- Better build system
- UART
- Safer GPIO

### Soon

- A basic shell?
- USB driver?
- Audio?

### Reach

- Graphics?
- Networking stack?

## Helpful links

[BCM2835 ARM Peripherals](https://www.raspberrypi.org/documentation/hardware/raspberrypi/bcm2835/BCM2835-ARM-Peripherals.pdf)
[Raspberyy Pi B+ Schematic](https://www.raspberrypi.org/documentation/hardware/raspberrypi/schematics/Raspberry-Pi-B-Plus-V1.2-Schematics.pdf)