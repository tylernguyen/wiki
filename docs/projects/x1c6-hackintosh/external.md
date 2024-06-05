# External

## ACPI, ASL, and Patches

- The patches written for this project are in ASL. Consder reading the [ACPI Source Language (ASL) Tutorial v20190625](https://acpica.org/sites/acpica/files/asl_tutorial_v20190625.pdf) to get a basic understanding of the patches' code.

/// info
The Ubuntu Wiki also has an [ACPI Tricks and Tips](https://wiki.ubuntu.com/Kernel/Reference/ACPITricksAndTips) section.
///

- [5T33Z0/OC-Little-Translated](https://github.com/5T33Z0/OC-Little-Translated) is the English docs translation of [daliansky/OC-little](https://github.com/daliansky/OC-little). It is helpful to refer to existing patches when Hackintoshing.

/// warning
Some patches within OC-Little can be oudated, badly done, or fragmented because of different patch authors. Consider using this resource only as a reference and basic guide, not a patch repository.
///
- Consider referencing the [MacbookPro14,1 ACPI Dump](https://github.com/khronokernel/DarwinDumped/tree/master/MacBookPro/MacBookPro14%2C1) when trying to understand certain functions within macOS.

## Acidanthera Official Docs

- Consider reading `Configuration.pdf` from the OpenCore release package if you haven't. From there, pay attention to `Differences.pdf` with everynew OpenCore releases.

- WhateverGreen Intel HD Graphics FAQ: [WhateverGreen/Manual/FAQ.IntelHD.en.md](https://github.com/acidanthera/WhateverGreen/blob/master/Manual/FAQ.IntelHD.en.md)

## UEFI Secure Boot

It is possible to enable Secure Boot with macOS. Doing so will require custom secure boot keys and signing OpenCore binaries each update. See [profzei/Matebook-X-Pro-2018/wiki](https://github.com/profzei/Matebook-X-Pro-2018/wiki/Enable-BIOS-Secure-Boot-with-OpenCore) for a basic getting started guide.

/// info
UEFI Secure Boot Explanation: [hac-mini-guide/details/secure-boot](https://osy.gitbook.io/hac-mini-guide/details/secure-boot)
///

## Thunderbolt 3

[osy](https://github.com/osy) has a great write-up of patching Thunderbolt 3 hotplug under macOS. See [Part 1](https://osy.gitbook.io/hac-mini-guide/details/thunderbolt-3-fix), [Part 2]( https://osy.gitbook.io/hac-mini-guide/details/thunderbolt-3-fix-part-2), and [Part 3](https://osy.gitbook.io/hac-mini-guide/details/thunderbolt-3-fix-part-3).
