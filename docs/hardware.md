---
icon: material/harddisk
tags:
  - Evergreen
---

# Hardware

## Computers

/// abstract | Philosophy
I like full-sized form factor builds for expandability, ease of maintenance, and generally cheaper and more available used parts.

Similarly, I prefer air-cooling over water-cooling for better reliability and repairability.

And I passionately hate RGBs!
///

/// tab | Desktop PC
My PC runs ![Windows 11](https://assets.tylernguyen.wiki/logos/Windows11.svg){ .twemoji } Windows 11 and is mostly used for gaming.

- __BenQ Zowie XL2566K__

I typically play :simple-valorant:{ .valorant } VALORANT so the 25" size and 360Hz refresh rate goes well together. I don't recommend this monitor, however, as it is 1080p and a TN panel. My dream monitor would be a 25" 1440p OLED at 360Hz.

- __GIGABYTE X570S AORUS Master__
- __AMD Ryzen 7 5800X3D__
- __Noctua NH-D15 chromax.Black__

_AM4_ is more than adequate for my fidelity and performance needs right now. I don't intend to upgrade to _AM5_. The next platform upgrade would likely be AM6 or Intel's equivalent.

- __Fractal Torrent__
- __EVGA RTX 3080 Ti FTW3 Ultra__
- __Sabrent Rocket 4.0 Plus 1TB__
- __Crucial P3 3.0 4TB__
- __be quiet! Dark Power 12 1000W__
///

/// tab | Server
My home server runs :simple-unraid:{ .unraid } Unraid. The primary usage is for media archival and consumption. It also hosts my :simple-homeassistant:{ .homeassistant } Home Assistant, :simple-forgejo:{ .forgejo } Forgejo, and :simple-mastodon:{ .mastodon } Mastodon instance. See [.wiki/self-hosted :octicons-arrow-down-left-16:](self-hosted.md).

- __Fractal Meshify 2 XL__

I maxed out this case with 20 3.5" drives. I'll start to rotate out older and smaller capacity drives on upgrades for next few years. On the next platform upgrade (in ~5 years), I'll probably move to a rackmounted form factor.

- __ASRock X570 Phantom Gaming X__
- __AMD Ryzen 9 3950X__
- __Noctua NH-D15 chromax.Black__
- __PNY RTX 4000__
- __Micron 32GB DDR4-3200 ECC UDIMM 2Rx8 CL22 MTA18ASF4G72AZ-3G2R__
- __178TB of mixed 3.5" drives__: retail, shucked, and used

Main data array (150TB), formatted in XFS and runs with 2 drives (_2x_ 14TB) as parities.

  [Disk Prices (US)](https://diskprices.com/) is convenient price checking/tracking tool for drive prices.

- _2x_ __1TB WD SN750 NVMes__

Primary cache that holds app and configuration data. They are formmatted in :simple-openzfs:{ .openzfs } ZFS and run in RAID1

- _2x_ __2TB Crucial MX500 2.5"__

Secondary cache used for temporary data and faster decrompression. They are formated in btrfs and run in RAID0.

- __be quiet! Dark Power 12 1000W__
///

/// tab | Laptops

- __Apple 14" Macbook Pro M3 Max__, 36GB unified memory

This is my de-facto workhorse. The hardware and form factor is perfect for my use case. I plan on renewing AppleCare for it when it expires and don't intend on upgrading for the foreseeable future.

- __Lenovo Thinkpad X1C6__

This was my old laptop and used for about 6 years. It runs :material-apple-finder: macOS, see [.wiki/projects/x1c6-hackintosh](projects/x1c6-hackintosh/README.md).
///

## Mobile

- __iPhone 14 Pro__

It's an iPhone: nothing more, nothing less. It's much more powerful than what I use it for, especially since I don't care for photos. The battery life is what matters most to me. Should Apple releases a new iPhone Mini, I'd likely swap to that.

- __iPad Mini 6th Gen__

I use the iPad Mini to read the web, comics, mangas, and the occasional textbooks. It's also how I watch movies and shows on the treadmill.

- __Kobo Clara BW__

This is my default device for reading books. And since the majority of my book-reading are before bedtime, it lives primarily on my headboard or nightstand.

Runs :octicons-git-branch-16:{ .foreground } [koreader/koreader](https://github.com/koreader/koreader)
    ![GitHub Stars](https://img.shields.io/github/stars/koreader/koreader?style=flat&logo=GitHub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
    ![GitHub Forks](https://img.shields.io/github/forks/koreader/koreader?style=flat&logo=GitHub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
    ![GitHub Stars](https://img.shields.io/github/stars/koreader/koreader?style=flat&logo=GitHub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }
    ![GitHub Forks](https://img.shields.io/github/forks/koreader/koreader?style=flat&logo=GitHub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }

## Consoles

- __Steam Deck OLED LE__

I love my Steam Deck OLED. I previously had a standard Steam Deck and cannot recommend the OLED model enough. I use it at my desk, in bed, and on travel. I play mostly indie and emulated titles on it.

- __Nintendo Switch OLED__

This is solely for Nintendo exclusive games.

- __ANBERNIC RG35XXSP__

I use this to mostly play Pokemon ROM hacks.

Runs [MuOS](https://muos.dev/) instead of the stock operating system.

## Miscellaneous

- __Apple AirTag__
- __Yubikey 5C__

/// tip
Yubikey can also be used for :simple-gnuprivacyguard:{ .gnuprivacyguard } GnuPG and SSH.

See :octicons-git-branch-16:{ .foreground } [drduh/YubiKey-Guide](https://github.com/drduh/YubiKey-Guide)
    ![GitHub Stars](https://img.shields.io/github/stars/drduh/YubiKey-Guide?style=flat&logo=GitHub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
    ![GitHub Forks](https://img.shields.io/github/forks/drduh/YubiKey-Guide?style=flat&logo=GitHub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
    ![GitHub Stars](https://img.shields.io/github/stars/drduh/YubiKey-Guide?style=flat&logo=GitHub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }
    ![GitHub Forks](https://img.shields.io/github/forks/drduh/YubiKey-Guide?style=flat&logo=GitHub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }
///
