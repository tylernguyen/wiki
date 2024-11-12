---
icon: material/chip
---

# BIOS Settings

## BIOS Modding

Modding the machine's BIOS is __optional__ and will unlock hidden advanced settings. These settings allow for better optimizations under macOS.

/// danger
The BIOS patch will <span class="solarized-red">__PERMANENTLY__</span> break TPM. Patch the only BIOS if you (will) never use TPM under Windows or Linux.
///

The CH341a SPI Programmer and SOIC8 Clip are needed to dump and flash the BIOS chip. An inexpensive one from Amazon/eBay is sufficient.

The BIOS chip is located just above the CPU, hidden under the shielding sticker.

<figure markdown>
  ![BIOS Chip Location](https://user-images.githubusercontent.com/3349081/87883762-38686380-c9cf-11ea-9e9d-c400f7b5407b.jpg){ loading-lazy width=300 }
  <figcaption>X1C6 BIOS Chip Location</figcaption>
</figure>

<div class="grid cards" markdown>

- :octicons-git-branch-16:{ .foreground } [digmorepaka/thinkpad-firmware-patches](https://github.com/digmorepaka/thinkpad-firmware-patches)
    ![GitHub Stars](https://img.shields.io/github/stars/digmorepaka/thinkpad-firmware-patches?style=flat&logo=GitHub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
    ![GitHub Forks](https://img.shields.io/github/forks/digmorepaka/thinkpad-firmware-patches?style=flat&logo=GitHub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
    ![GitHub Stars](https://img.shields.io/github/stars/digmorepaka/thinkpad-firmware-patches?style=flat&logo=GitHub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }
    ![GitHub Forks](https://img.shields.io/github/forks/digmorepaka/thinkpad-firmware-patches?style=flat&logo=GitHub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }

</div>

/// announce | Credits
Thank you to `paranoidbashthot` and `\x` for creating the patches.
///

[:simple-youtube:{ .youtube } @notthebee](https://github.com/notthebee) similarly modded his BIOS in [:simple-youtube:{ .youtube } Removing Wi-Fi Whitelist ... & Unlocking Advanced BIOS Settings](https://www.youtube-nocookie.com/embed/ce7kqUEccUM)

1. Use `xx_80_patches-v*.txt`, feel free to comment out the WWAN patches if unnecessary.

3. Remember to __dump the vanilla twice and use `diff` to make sure things were dumped properly__, store this backup somewhere safe.
4. Confirmed working `BIOS-v1.45`, I cannot be sure about other BIOS versions. Though they will most likely work as well.
5. The modded BIOS does not need to be signed by `thinkpad-eufi-sign`. Remember to replace `4C 4E 56 42 42 53 45 43 FB` with `4C 4E 56 42 42 53 45 43 FF` on the patched BIOS.

6. Your BIOS chip may not be made by Winbond, but by Macronix instead. In that case, add the argument `-c MX25L12835F/MX25L12845E/MX25L12865E` to `flashrom`. See [Issue #116](https://github.com/tylernguyen/x1c6-hackintosh/issues/116#issuecomment-778654320)

/// success
Successfully modding your BIOS will reveal the __Advanced__ tab.

<p align="center">
<img align="center" src="https://user-images.githubusercontent.com/3349081/87883767-3d2d1780-c9cf-11ea-9fb0-f250590a3f28.jpg" alt="BIOS Advance Menu" width="300">
</p>

It is safe to update the BIOS. However, the patches will have to be reapplied and reflashed.
///

## Modded BIOS Settings

- DVMT Pre-Allocated to `64M`. This enables 4K HDMI output.
- Disable CFG Lock. This gives Kernel (XNU) and AppleIntelPowerManagement the ability to write to the MSR 0xE2 register.

## Vanilla BIOS Settings

The following settings are not all necessary, but are recommended for general compatibility and stability.

- Disable TPM
- Disable Secure Boot
- Disable Fingerprint Reader
- 'UEFI Only' Boot
- Disable CSM Support
- Disable Wke on LAN

## Thunderbolt 3

Thunderbolt 3 hot-plug support under macOS noticeably increases the idle power consumption.

- Disable Thunderbolt BIOS Assist Mode
- Security Level to `No Security`
- Disable Support in Pre Boot Environment

If you don't use Thunderbolt 3 or prioritize power consumption, you can still cold-plug Thunderbolt 3.

- Enabled Thunderbolt BIOS Assist Mode
- Enable Thunderbolt Device
