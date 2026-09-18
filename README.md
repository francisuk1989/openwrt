![OpenWrt logo](include/logo.png)

Custom OpenWrt development builds for the **AVM FRITZ!Box 7530 non-AX (HW236 rev2)**.

These builds are based on https://github.com/openwrt/openwrt and are primarily intended for development, testing, and hardware investigation.

## FRITZ!Box 7530 non-AX HW236 rev2

## Experimental Status

These are **experimental development builds**.

The FRITZ!Box 7530 non-AX HW236 rev2 work currently includes hardware features that are still being investigated, particularly:

- GPIO31 LED function and polarity
- IPQ4019 ADSS PWM support
- Qualcomm QCE/AES acceleration
- Factory DSL/WAN MAC handling through AVM TFFS3 `macdsl`

RAM booting is preferred while testing experimental hardware changes.

**AVM FRITZ!Box 7530 AX (HW256)**.
**uses a Broadcom BCM63178 platform**
> [!WARNING]
> OpenWrt dos not have support for the BCM63178
> Do not flash images to NAND unless you understand the recovery procedure, and risks involved.
---

---

## Project Goals

The aim of this project is to investigate and develop OpenWrt support
for the FRITZ!Box 7530 AX while preserving the original AVM firmware
and factory data.

Current areas of investigation include:

- Broadcom BCM63178 platform support
- AVM HW256 device tree
- NAND partition layout
- AVM TFFS factory/configuration storage
- Dual FIT firmware layout
- Boot-slot selection
- Ethernet
- DSL
- Wi-Fi
- LEDs and buttons
- GPIOs
- USB
- Factory MAC addresses
- Safe OpenWrt boot and recovery methods
