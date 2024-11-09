---
icon: octicons/gear-16
---

# Post Install

## YogaSMC

<div class="grid cards" markdown>

- :octicons-git-branch-16:{ .foreground } [zhen-zen/YogaSMC](https://github.com/zhen-zen/YogaSMC)
    ![GitHub Stars](https://img.shields.io/github/stars/zhen-zen/YogaSMC?style=flat&logo=GitHub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
    ![GitHub Forks](https://img.shields.io/github/forks/zhen-zen/YogaSMC?style=flat&logo=GitHub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
    ![GitHub Stars](https://img.shields.io/github/stars/zhen-zen/YogaSMC?style=flat&logo=GitHub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }
    ![GitHub Forks](https://img.shields.io/github/forks/zhen-zen/YogaSMC?style=flat&logo=GitHub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }

    - YogaSMCPane is the preference pane showing basic information and settings.
    - YogaSMCNC is the notification app that receive EC events. It also has fan control.

</div>

## HiDPI Display

/// warning
Enabling HiDPI requires disabling Apple's System Integrity Protection (SIP).
///

/// danger
Users of `SecureBootModel` may end up in a RecoveryOS boot loop if the system partition has been modified. To resolve this, Reset NVRAM and set `SecureBootModel` to `Disabled`
///

1. Disable SIP. I prefer to use `ToggleSipEntry.efi` at Boot Picker.
2. Mount drive as writeable. See [instructions](https://dortania.github.io/OpenCore-Install-Guide/troubleshooting/extended/post-issues.html#writing-to-the-macos-system-partition)
3. Run [xzhih/one-key-hidpi](https://github.com/xzhih/one-key-hidpi)
    - for Ventura: use this fork [yurhett/one-key-hidpi](https://github.com/yurhett/one-key-hidpi)
4. Enable SIP.

## HDMI Out

### EDID Override

- This is necessary to fix HDMI hotplug.
- See current available patches in `/patches/Internal Displays/`, merge them with `config.plist`
- If a patch is not yet created for your display model. Please see [Issue #60](https://github.com/tylernguyen/x1c6-hackintosh/issues/60) to create your own EDID override. Please create a pull request to add your EDID override for different displays.

## Dual Booting

I recommend that you dual boot using another drive in the WWAN slot (I have the WDC PC SN520 NVMe 2242). This makes installation much easier, and lets the BIOS F12 option act as your boot manager.

/// note
Lenovo's Boot Manager will not have an entry for the WWAN NVMe. Most OS(es) will create a bootloader entry during install. If not, use OpenCore to boot into these partitions. See [dortania / OpenCore-Multiboot](https://dortania.github.io/OpenCore-Multiboot/)
///

/// tip
It is possible to share Bluetooth pairing keys between Windows and macOS when dual booting.

The `.reg` for Bluetooth connected devices in macOS can be exported using Hackintool's Utilities section. This key can then be imported to Windows.
///

## iMessage and other Apple Services

- Refer to [dortania /OpenCore-Install-Guide](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html)

/// note
`We’re sorry, but this serial number isn’t valid` is fine and has personally worked and working for me and many others. `Purchase Date not Validated` can be a problem down the line if a legitimate machine with that PlatformInfo is activated.
///

## Keyboard

/// note
MultiMedia Fn keys will work out of the box. Special Fn keys require [YogaSMC App](https://github.com/zhen-zen/YogaSMC) to be installed. Additionally, some parameters can be configured with YogaSMC's PrefPane plugin.
///

- PrtSc (remapped to F13) = I use it for Screen Capture (Set in `System Preferences/Keyboard/Shortcuts`)
- Check `Use F1, F2, etc. keys as standard function keys` in `System Preferences/Keyboard` to gain access to standard F keys:

<p align="center">
  <img src="https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/keyboard.png" width="500">
</p>

/// tip
[Karabiner-Elements](https://karabiner-elements.pqrs.org/) and [BetterTouchTool](https://folivora.ai/) are great advanced customization tools for your keyboard.
///

## Sleep

- Disable Power Nap for both [`Battery`](https://github.com/tylernguyen/x1c6-hackintosh/blob/main/docs/assets/macOS%20Settings/Battery_powernap.png) and [`Power Adapter`](https://github.com/tylernguyen/x1c6-hackintosh/blob/main/docs/assets/macOS%20Settings/Poweradt_powernap.png).
- Disable [`Wake for Network Access`](https://github.com/tylernguyen/x1c6-hackintosh/blob/main/docs/assets/macOS%20Settings/Poweradt_powernap.png) in `Power Adapter`.

- Uncheck `Allow Bluetooth devices to wake this computer` if you do not need it.

<p align="center">
  <img src="https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/bluetooth.png" width="500">
</p>

- Do not disable `hibernatefile`.
- `sudo pmset -a tcpkeepalive 0` to disable Network while sleeping.
- `sudo pmset -a proximitywake 0` to disable peripheral wake agent.

## Thunderbolt 3

- Native-like integration with macOS in System Report without the need of flashing a modded firmware. Thank you [@benbender](https://github.com/benbender)
- NOTE: If you do have a modded BIOS firmware, please reset all settings relating to Thunderbolt 3 to default, all that's needed are settings detailed below or in [Settings for Vanilla BIOS](https://tylernguyen.github.io/x1c6-hackintosh/BIOS/settings-for-vanilla-BIOS/)
- Please make sure of these settings in BIOS:

| Main Menu | Sub 1       | Sub 2                                         | Sub 3                                                              |
| --------- | ----------- | --------------------------------------------- | ------------------------------------------------------------------ |
|           | >> Config   | >> Thunderbolt (TM) 3                         | Thunderbolt BIOS Assist Mode `Disabled`                            |
|           |             |                                               | Security Level `No Security`                                       |
|           |             |                                               | Support in Pre Boot Environment: Thunderbolt(TM) Device `Disabled` |

/// warning
USB 3.1 Gen2 hotplug will likely never work. It is also neither planned nor currently worked on. If you need USB 3.1 Gen2, coldboot the machine with the device attached.
///

## Trackpad

- Force Click is enabled by default, which turns any click on the trackpad into a force touch. I suggest you turn this off.
- In addition, I prefer to have tap to click on:

<p align="center">
  <img src="https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/trackpad.png" width="500">
</p>
