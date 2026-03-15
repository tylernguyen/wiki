---
icon: material/harddisk
tags:
  - evergreen
  - uses
---

# Hardware

> [!danger] Lighting
> I hate decorative RGBs. They're a distraction, waste of money and energy.

## Desktop

Runs ![Windows 11](https://assets.tylernguyen.wiki/logos/Windows11.svg){ .twemoji } Windows 11 and is mostly used for gaming.

- __Monitor__: BenQ Zowie XL2566K

I typically play :simple-valorant:{ .valorant } VALORANT so the 25" size and 360Hz refresh rate goes well together. I don't recommend this monitor, however, as it is 1080p and a TN panel. My dream monitor would be a 25" 1440p OLED at 360Hz.

- __Case__: Fractal Torrent

I like full-sized form factor builds for expandability, ease of maintenance, and generally cheaper and more available used parts.

- __MOBO__: GIGABYTE X570S AORUS Master
- __CPU__: AMD Ryzen 7 5800X3D

_AM4_ is more than adequate for my fidelity and performance needs right now. I don't intend to upgrade to _AM5_. The next platform upgrade would likely be AM6 or Intel's equivalent.

- __CPU Cooler__: Noctua NH-D15 chromax.Black
- __GPU__: EVGA RTX 3080 Ti FTW3 Ultra
- __NVMe__: Sabrent Rocket 4.0 Plus 1TB
- __NVMe__: Crucial P3 3.0 4TB
- __PSU__: be quiet! Dark Power 12 1000W

## Server

Runs :simple-unraid:{ .unraid } Unraid, the primary usage is for media archival and consumption.

__See [.wiki/self-hosted :lucide-arrow-down-left:](self-hosted.md) for my software stack.__

- __Case__: Fractal Meshify 2 XL

I maxed out this case with 20 3.5" drives. I'll start to rotate out older and smaller-capacity drives over the next few years. On the next platform upgrade (in ~5 years), I'll probably move to a rackmounted form factor.

- __MOBO__: ASRock X570 Phantom Gaming X
- __CPU__: AMD Ryzen 9 3950X
- __CPU Cooler__: Noctua NH-D15 chromax.Black
- __GPU__: PNY RTX 4000
- __RAM__: 128GB (4x Micron 32GB DDR4-3200 ECC UDIMM 2Rx8 CL22 MTA18ASF4G72AZ-3G2R)
- __HDD__: 186TB of mixed 3.5" drives (retail, refurb, schucked, used)

Main data array (158TB usable) is formatted in XFS and runs with 2 drives (_2x_ 14TB) as parities.

- __NVMe Cache__: 2x 1TB WD SN750

Primary cache for Docker appdata, formatted in :simple-openzfs:{ .openzfs } ZFS and run in RAID1.

- __SATA Cache__: 2x 2TB Crucial MX500 2.5"

Secondary cache used for temporary data and faster decompression, formatted in btrfs and run in RAID0.

- __PSU__: be quiet! Dark Power 12 1000W

## Mobile

- :simple-apple:{ .foreground} __Apple 14" Macbook Pro M3 Max__, 36GB unified memory

This is my de-facto workhorse. The hardware and form factor is perfect for my use case. I plan on renewing AppleCare for it when it expires and don't intend on upgrading for the foreseeable future.

- :simple-apple:{ .foreground} __iPhone 14 Pro__

It's an iPhone: nothing more, nothing less. It's much more powerful than what I use it for, especially since I don't care for photos. The battery life is what matters most to me. Should Apple release a new iPhone Mini, I'd likely swap to that.

- :simple-apple:{ .foreground} __iPad Mini 6th Gen__

I use the iPad Mini to read the web, comics, mangas, and the occasional textbooks. It's also how I watch movies and shows on the treadmill.

- __Kobo Clara BW__

This is my default device for reading books. And since the majority of my book-reading are before bedtime, it lives primarily on my headboard or nightstand.

Runs :simple-koreader:{ .koreader } [KOReader :lucide-arrow-up-right:](https://github.com/koreader/koreader).

## Consoles

- :simple-steamdeck:{ .steamdeck } __Steam Deck OLED LE__

I love my Steam Deck OLED. I previously had a standard Steam Deck and cannot recommend the OLED model enough. I often use it in bed, and during travel. On it, I mostly play roguelikes and emulated titles.

- ![Nintendo Switch](https://assets.tylernguyen.wiki/logos/Nintendo_Switch.svg){ .twemoji } __Nintendo Switch OLED__

This is solely for Nintendo exclusive games. Nintendo games are particularly good for

See [/favorites#games :lucide-arrow-down-left:](favorites.md#games)

## Home Network

- :simple-ubiquiti:{ .ubiquiti } __Ubiquiti UniFi Cloud Gateway Fiber__

I get ~2Gbps symmetrical from my fiber provider. It's more than adequate for my household usage. So my network is designed with 2.5GbE in mind. I don't foresee upgrading to a 10GbE setup even in the far future.

- :simple-ubiquiti:{ .ubiquiti } __Ubiquiti UniFi U7 Pro XG__

I only use 1 AP for the house and try to keep the number of Wi-Fi connected devices to a minimum. I recently just upgraded to the U7 Pro XG and it's been stable thus far. I don't plan upgrading anytime soon.

- :simple-ubiquiti:{ .ubiquiti } __Ubiquiti Unifi Flex 2.5G 5__

This switch is mostly used for gaming devices. They usually saturate the speed during downloads.

- :simple-ubiquiti:{ .ubiquiti } __Ubiquiti UniFi USW-Lite-8-PoE__

The majority of my PoE devices are low bandwidth. As long as my setup doesn't include a PoE device that needs more than 1 gigabit. There are no reasons to upgrade.

## Miscellaneous

- :simple-apple:{ .foreground} __Apple AirTag__
- :simple-yubico:{ .yubico } __Yubikey 5C NFC__

I use the Yubikey as 2FA and/or passkey for a few critical accounts. It's also apart of my GnuPG workflow. But :simple-1password:{ .onepassword } 1Password handles most of my daily security.

See :lucide-folder-git-2:{ .foreground } [drduh/YubiKey-Guide :lucide-arrow-up-right:](https://github.com/drduh/YubiKey-Guide).
