---
icon: material/harddisk
tags:
  - evergreen
  - uses
---

# Hardware

/// danger | Lighting
I hate decorative RGBs. They're a distraction, waste of money and energy.
///

## Computers

/// tab | Desktop :lucide-monitor:{ style="margin-right: 0" }:lucide-pc-case:{ style="margin-left: 0" }
My PC runs ![Windows 11](https://assets.tylernguyen.wiki/logos/Windows11.svg){ .twemoji } Windows 11 and is mostly used for gaming.

- __BenQ Zowie XL2566K__

I typically play :simple-valorant:{ .valorant } VALORANT so the 25" size and 360Hz refresh rate goes well together. I don't recommend this monitor, however, as it is 1080p and a TN panel. My dream monitor would be a 25" 1440p OLED at 360Hz.

- __Fractal Torrent__
I like full-sized form factor builds for expandability, ease of maintenance, and generally cheaper and more available used parts.

- __GIGABYTE X570S AORUS Master__
- __AMD Ryzen 7 5800X3D__
- __Noctua NH-D15 chromax.Black__

_AM4_ is more than adequate for my fidelity and performance needs right now. I don't intend to upgrade to _AM5_. The next platform upgrade would likely be AM6 or Intel's equivalent.

- __EVGA RTX 3080 Ti FTW3 Ultra__
- __Sabrent Rocket 4.0 Plus 1TB__
- __Crucial P3 3.0 4TB__
- __be quiet! Dark Power 12 1000W__
///

/// tab | Server :lucide-server:
My home server runs :simple-unraid:{ .unraid } Unraid. The primary usage is for media archival and consumption.

__See [.wiki/self-hosted :octicons-arrow-down-left-16:](self-hosted.md) for more details on my self-hosted stack.__

- __Fractal Meshify 2 XL__

I maxed out this case with 20 3.5" drives. I'll start to rotate out older and smaller-capacity drives over the next few years. On the next platform upgrade (in ~5 years), I'll probably move to a rackmounted form factor.

- __ASRock X570 Phantom Gaming X__
- __AMD Ryzen 9 3950X__
- __Noctua NH-D15 chromax.Black__
- __PNY RTX 4000__
- ___128GB___ of 4x __Micron 32GB DDR4-3200 ECC UDIMM 2Rx8 CL22 MTA18ASF4G72AZ-3G2R__
- ___186TB___ of __mixed 3.5" drives__: retail, refurb, schucked, used.

Main data array (158TB usable) is formatted in XFS and runs with 2 drives (_2x_ 14TB) as parities.

- _2x_ __1TB WD SN750 NVMes__

Primary cache that holds app and configuration data. They are formatted in :simple-openzfs:{ .openzfs } ZFS and run in RAID1.

- _2x_ __2TB Crucial MX500 2.5"__

Secondary cache used for temporary data and faster decompression. They are formatted in btrfs and run in RAID0.

- __be quiet! Dark Power 12 1000W__
///

/// tab | Laptop :lucide-laptop:

- __Apple 14" Macbook Pro M3 Max__, 36GB unified memory

This is my de-facto workhorse. The hardware and form factor is perfect for my use case. I plan on renewing AppleCare for it when it expires and don't intend on upgrading for the foreseeable future.
///

## Mobile

- __iPhone 14 Pro__

It's an iPhone: nothing more, nothing less. It's much more powerful than what I use it for, especially since I don't care for photos. The battery life is what matters most to me. Should Apple release a new iPhone Mini, I'd likely swap to that.

- __iPad Mini 6th Gen__

I use the iPad Mini to read the web, comics, mangas, and the occasional textbooks. It's also how I watch movies and shows on the treadmill.

- __Kobo Clara BW__

This is my default device for reading books. And since the majority of my book-reading are before bedtime, it lives primarily on my headboard or nightstand.

Runs :octicons-git-branch-16:{ .foreground } [koreader/koreader :octicons-arrow-up-right-16:](https://github.com/koreader/koreader)
    ![GitHub Stars](https://img.shields.io/github/stars/koreader/koreader?&style=flat&logo=GitHub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
    ![GitHub Forks](https://img.shields.io/github/forks/koreader/koreader?&style=flat&logo=GitHub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
    ![GitHub Stars](https://img.shields.io/github/stars/koreader/koreader?&style=flat&logo=GitHub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }
    ![GitHub Forks](https://img.shields.io/github/forks/koreader/koreader?&style=flat&logo=GitHub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }

## Consoles

- __Steam Deck OLED LE__

I love my Steam Deck OLED. I previously had a standard Steam Deck and cannot recommend the OLED model enough. I use it at my desk, in bed, and on travel. I play mostly indie and emulated titles on it.

- __Nintendo Switch OLED__

This is solely for Nintendo exclusive games.

## Miscellaneous

- __Apple AirTag__
- __Yubikey 5C NFC__

/// tip
Yubikey can also be used for :simple-gnuprivacyguard:{ .gnuprivacyguard } GnuPG and SSH.

See :octicons-git-branch-16:{ .foreground } [drduh/YubiKey-Guide](https://github.com/drduh/YubiKey-Guide)
    ![GitHub Stars](https://img.shields.io/github/stars/drduh/YubiKey-Guide?&style=flat&logo=GitHub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
    ![GitHub Forks](https://img.shields.io/github/forks/drduh/YubiKey-Guide?&style=flat&logo=GitHub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
    ![GitHub Stars](https://img.shields.io/github/stars/drduh/YubiKey-Guide?&style=flat&logo=GitHub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }
    ![GitHub Forks](https://img.shields.io/github/forks/drduh/YubiKey-Guide?&style=flat&logo=GitHub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }
///


## Home Network :material-ethernet:

- __Ubiquiti UniFi Cloud Gateway Fiber__

I get ~2Gbps symmetrical from my fiber provider. It's more than adequate for my household usage. So my network is designed with 2.5GbE in mind. I don't foresee upgrading to a 10GbE setup even in the far future.

- __Ubiquiti UniFi U7 Pro XG__

I only use 1 AP for the house and try to keep the number of Wi-Fi connected devices to a minimum. I recently just upgraded to the U7 Pro XG and it's been stable thus far. I don't plan upgrading anytime soon.

- __Ubiquiti Unifi Flex 2.5G 5__

This switch is mostly used for gaming devices. They usually saturate the speed during downloads.

- __Ubiquiti UniFi USW-Lite-8-PoE__

The majority of my PoE devices are low bandwidth. As long as my setup doesn't include a PoE device that needs more than 1 gigabit. There are no reasons to upgrade.
