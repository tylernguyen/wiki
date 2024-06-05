---
icon: material/apple-finder
---

# Install macOS

## Create the Installer

Start by creating a vanilla macOS installer, refer to [Dortania's Creating the USB](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/).

You may also use [`createinstallmedia`](https://support.apple.com/en-us/101578) if you already have a Mac.

/// tip
Often as above, the project will defer universal steps to Dortania links. Hence, this repository is meant to be used in conjunction with their guides.
///

## Prep the Installer

![OpenCore](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/OpenCore.png){ align=right width=100 }

/// warning
The default EFI folder is BIOS and network card agnostic.
///

Vanilla BIOS: merge `/patches/ OpenCore Patches/ Vanilla BIOS.plist` with `config.plist`

Intel Network Cards [![OpenIntelWireless](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/OpenIntelWireless.png){ .twemoji }  OpenIntelWireless](<https://openintelwireless.github.io/>)

\*Notice that these patches require additional kexts to be installed. See them in `Kernel/Add/`

1. Make the following changes to `config.plist` within the `EFI` folder.
    - `ShowPicker` to `YES`
    - `ScanPolicy` to `0`
2. Mount the installer media's EFI partition. You may do this via the command line with `diskutil` or via a utility like [corpnewt/MountEFI](https://github.com/corpnewt/MountEFI).
3. Copy the EFI folder into the installer media's EFI partition. Remember that the top directory level should be `EFI`.
4. Boot into the macOS installer environment using the media. Format target disk as `APFS` using `Disk Utility` and complete installation.

## First Boot

1. Boot the installed macOS partition with the existing installer USB and complete new user setup.
2. Copy `EFI` from the installer into the macOS drive's EFI partition. Set `ShowPicker` to `NO` for a cleaner boot experience. You can still access the boot picker by pressing `ESC` during boot time.

/// success
Your machine should now be able to independently boot macOS.
///
