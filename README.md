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

https://github.com/francisuk1989/openwrt/blob/main/target/linux/bmips/dts/bcm63178-avm-fritzbox-7530-ax.dts

Experimental OpenWrt development and hardware research for the

> [!WARNING]
> This project is experimental.
>
> Do not flash images to NAND unless you understand the boot layout,
> recovery procedure, and risks involved.
>
> Preserve a complete backup of the original flash before making
> persistent changes.

---

## Device

| Component | Details |
|---|---|
| Manufacturer | AVM |
| Model | FRITZ!Box 7530 AX |
| AVM Hardware ID | HW256 |
| HWRevision | 256 |
| HWSubRevision | 4 |
| Product ID | `Fritz_Box_HW256` |
| SoC | Broadcom BCM63178 |
| RAM | 512 MiB |
| NAND | 128 MiB |
| NAND erase size | 128 KiB |
| Boot layout | Dual FIT firmware slots |

The FRITZ!Box 7530 AX is substantially different from the original
FRITZ!Box 7530 non-AX (HW236).

The **7530 AX / HW256 uses a Broadcom BCM63178 platform** and should
therefore not be confused with the Qualcomm IPQ4019-based HW236.

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
