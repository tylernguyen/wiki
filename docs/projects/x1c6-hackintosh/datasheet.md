---
icon: material/data-matrix
---

# Datasheet

## Non-Functional

| Feature | Dependency | Remarks |
|---|---|---|
| :octicons-x-16:{ .solarized-red } Apple Music Lossless (DRM) |  | iGPU is incompatible with Apple's Lossless DRM. Try using an external DAC. |
| :octicons-x-16:{ .solarized-red } Fingerprint Reader | `DISABLED` in BIOS to save power if not used in other OSes. |  |
| :octicons-x-16:{ .solarized-red } Wireless WAN | `DISABLED` in BIOS to save power if not used in other OSes. | Unable to investigate as I have no need and my model did not come with WWAN. |
| :octicons-x-16:{ .solarized-red } Load Apple's Graphics Micro Code (GuC) |  | See [Issue #103](https://github.com/tylernguyen/x1c6-hackintosh/issues/103). Will never work AFAIK due to inherent incompatibility. |

## Video and Audio

| Feature | Dependency | Remarks |
|---|---|---|
| :octicons-check-16:{ .solarized-green } Full Graphics Acceleration (QE/CI)   | ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } WhateverGreen |                 |
| :octicons-check-16:{ .solarized-green } Webcam | ![UEFI](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/UEFI.png){ .twemoji } SSDT-XHC1     |  |
| :octicons-check-16:{ .solarized-green } Audio Recording                      | ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } AppleALC      | Layout ID = 21  |
| :octicons-check-16:{ .solarized-green } Audio Playback                       | ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } AppleALC      | Layout ID = 21  |
| :octicons-check-16:{ .solarized-green } Automatic Headphone Output Switching | ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } AppleALC      | Layout ID = 21  |

## Power, Charge, Sleep and Hibernation

| Feature | Dependency | Remarks |
|---|---|---|
| :octicons-check-16:{ .solarized-green }  Battery Percentage Indication     | ![UEFI](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/UEFI.png){ .twemoji } SSDT-Battery <br> ![OpenCore](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/OpenCore.png){ .twemoji } `/patches/OpenCore Patches/Battery.plist`             |
| :octicons-check-16:{ .solarized-green } CPU Power Management (SpeedShift)          | ![UEFI](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/UEFI.png){ .twemoji } SSDT-PM <br> ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } CPUFriend <br> ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } CPUFriendDataProvider  | [CPUFriendFriend](https://github.com/corpnewt/CPUFriendFriend_) or [one-key-cpufriend](https://github.com/stevezhengshiqi/one-key-cpufriend).
| :octicons-check-16:{ .solarized-green } iGPU Power Management          | ![UEFI](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/UEFI.png){ .twemoji } SSDT-PM                   |
| :octicons-check-16:{ .solarized-green }  NVMe Drive Battery Management | ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } NVMeFix | In my experience, NVMe drives will drain more power than SATA drives.           |
| :octicons-check-16:{ .solarized-green } S3 Sleep  | ![UEFI](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/UEFI.png){ .twemoji } SSDT-Sleep | |
| :octicons-check-16:{ .solarized-green } Hibernation Mode 25            | ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } RTCMemoryFixup <br> ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } HibernationFixup  | Supported, macOS uses mode 3 by default. Change to mode 25 via `pmset`.     |
| :octicons-check-16:{ .solarized-green } Custom Charge Threshold       | ![UEFI](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/UEFI.png){ .twemoji } SSDT-EC <br> ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } [YogaSMC](https://github.com/zhen-zen/YogaSMC) <br> [YogaSMCPane](https://github.com/zhen-zen/YogaSMC) | Adjust with YogaSMCPane in System Preferences
| :octicons-check-16:{ .solarized-green } Fan Control                    | ![UEFI](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/UEFI.png){ .twemoji } SSDT-EC <br> ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } [YogaSMC](https://github.com/zhen-zen/YogaSMC) <br> [YogaSMC App](https://github.com/zhen-zen/YogaSMC)| Adjust with YogaSMC App.

## Input and Output

| Feature | Dependency | Remarks |
|---|---|---|
| :octicons-check-16:{ .solarized-green } WiFi | Native with BCM94360CS2 <br> [![OpenIntelWireless](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/OpenIntelWireless.png){ .twemoji }  OpenIntelWireless](https://openintelwireless.github.io/) for Intel cards | See `/patches/ Network Patches/` for patches. |
| :octicons-check-16:{ .solarized-green } Bluetooth | ![UEFI](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/UEFI.png){ .twemoji } SSDT-XHC1 <br> Native with BCM94360CS2 <br> [![OpenIntelWireless](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/OpenIntelWireless.png){ .twemoji }  OpenIntelWireless](https://openintelwireless.github.io/) for Intel cards | See `/patches/ Network Patches/` for patches. |
| :octicons-check-16:{ .solarized-green } Ethernet | ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } IntelMausi | Needs Lenovo Ethernet adapter: [Item page](https://www.lenovo.com/us/en/accessories-and-monitors/cables-and-adapters/adapters/CABLE-BO-Ethernet-Extension-Adapter-2/p/4X90Q84427) |
| :octicons-check-16:{ .solarized-green } HDMI hotplug | Custom EDID Override ![OpenCore](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/OpenCore.png){ .twemoji } `/patches/Internal Displays/` | Refer to [Issue #60](https://github.com/tylernguyen/x1c6-hackintosh/issues/60) if one does not exist already for your display. |
| :octicons-check-16:{ .solarized-green } 4K HDMI/DisplayPort Output **(Modded BIOS)** | BIOS `DMVT Pre-Allocated` to `64M` | See [BIOS Settings](BIOS.md) for information about modding the BIOS. |
| :octicons-check-16:{ .solarized-green } 4K HDMI/DisplayPort Output **(Vanilla BIOS)** |![OpenCore](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/OpenCore.png){ .twemoji } `/patches/OpenCore Patches/4K-Output-wo-BIOSmod.plist` |  |
| :octicons-check-16:{ .solarized-green } USB 2.0 <br> :octicons-check-16:{ .solarized-green } USB 3.0 <br> :octicons-check-16:{ .solarized-green } Micro SD Card Reader | ![UEFI](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/UEFI.png){ .twemoji } SSDT-XHC1 |  |
| :octicons-check-16:{ .solarized-green } USB 3.1 Coldboot <br> ⚠️ USB 3.1 Hotplug | ![UEFI](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/UEFI.png){ .twemoji } SSDT-TB-DSB2-XHC2 | USB 3.1 Gen2 hotplug will likely never work. It is also neither planned nor currently worked on. If you need USB 3.1 Gen2, coldboot the machine with the device attached. |
| :octicons-check-16:{ .solarized-green } USB Power Properties in macOS | ![UEFI](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/UEFI.png){ .twemoji } SSDT-XHC1 |  |
| :octicons-check-16:{ .solarized-green } Thunderbolt 3 Hotplug | ![UEFI](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/UEFI.png){ .twemoji } SSDT-TB-* | Native interface within System Report |

## Display, TrackPad, TrackPoint, and Keyboard

| Feature | Dependency | Remarks |
|---|---|---|
| :octicons-check-16:{ .solarized-green } Brightness Adjustments | ![UEFI](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/UEFI.png){ .twemoji } SSDT-PNLF <br> ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } WhateverGreen <br> ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } BrightnessKeys |  |
| :octicons-check-16:{ .solarized-green } HiDPI | [xzhih/one-key-hidpi](https://github.com/xzhih/one-key-hidpi) | Scaling issues post-sleep fixed with AAPL, ig-platform `BAAnWQ==` |
| :octicons-check-16:{ .solarized-green } TrackPoint | ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } VoodooPS2Controller |  |
| :octicons-check-16:{ .solarized-green } TrackPad |  ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } VoodooSMBus <br> ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } VoodooRMI |  |
| :octicons-check-16:{ .solarized-green } Built-in Keyboard | ![UEFI](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/UEFI.png){ .twemoji } SSDT-Keyboard <br> ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } VoodooPS2Controller | Optimizations recommended, see [`Post Installation`](post-install.md) |
| :octicons-check-16:{ .solarized-green } Multimedia Keys | ![Apple Kext](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Apple_kext.png){ .twemoji } BrightnessKeys <br> [YogaSMC App](https://github.com/zhen-zen/YogaSMC) |  |

## macOS Continuity

| Feature | Dependency | Remarks |
|---|---|---|
| :octicons-check-16:{ .solarized-green } iCloud, iMessage, FaceTime | Whitelisted Apple ID, Valid SMBIOS | See [dortania/OpenCore-Install-Guide](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html) |
| :octicons-check-16:{ .solarized-green } Continuity | Native with BCM94360CS2. `ExtendBTFeatureFlags` to `True` otherwise. | See `/patches/Network Patches/` for specific network card. |
| :octicons-check-16:{ .solarized-green } AirDrop | Native with BCM94360CS2. `ExtendBTFeatureFlags` to `True` otherwise. | See `/patches/Network Patches/` for specific network card. |
| :octicons-check-16:{ .solarized-green } Sidecar | Native with BCM94360CS2. `ExtendBTFeatureFlags` to `True` otherwise. iPad with >= `iPadOS 13` | Tested with iPad Mini with iPadOS 13.1.2 |
| :octicons-check-16:{ .solarized-green } FileVault | as configured in `config.plist` per [Dortania's Post-Install](https://dortania.github.io/OpenCore-Post-Install/universal/security/filevault.html) |  |
| :octicons-check-16:{ .solarized-green } Time Machine | Native | TimeMachine only backups your Macintosh partition. Manually backup your EFI partition using another method. |
