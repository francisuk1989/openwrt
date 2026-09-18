![OpenWrt logo](include/logo.png)

Custom builds for the **AVM FRITZ!Box 7530 non-AX (HW236 rev.2)**.

These builds are based on https://github.com/openwrt/openwrt and are primarily intended for development, testing, and hardware investigation.

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
