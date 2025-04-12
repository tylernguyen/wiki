# ACPI Patches

## ACPI Patches

1. Download and install [MaciASL](https://github.com/acidanthera/MaciASL/releases) if you do not have it already.
2. Dump your original ACPI tables. See [Dortania/ ACPI Dump](https://dortania.github.io/Getting-Started-With-ACPI/Manual/dump.html).
3. In Terminal, disassemble the copied ACPI tables with "iasl -dl DSDT.aml". For our purpose, the only file that really matters is DSDT.dsl

- Your DSDT file will be used as a reference table in determining that needs to be patched and what patches need to be added.

4. Source SSDT\*.dsl patch files are located in `patches` folder.
5. Refer to my `EFI-OpenCore` folder to see which patches are currently being used by me.
6. If your x1c6's model is 20KH*, most of my compiled hotpatches and can likely be copied straight to your setup. However, some patches may require certain directories or variables to be changed depending on your hardware (examine your own disassemebled DSDT). For these, edit the .dsl patch files. Also, note that some SSDT patches also require accompanying OpenCore/ Clover ACPI patches to work.

A good way to see if you need to edit and compile your own SSDT patches is to compare your DSDT.dsl with mine of the same BIOS version. You can find my disassemebled DSDT file in `ACPI/Disassembled ACPI/BIOS-v*`.

Should your source DSDT be similar enough (in regards to certain items in these ACPI patches)to mine. Congrats! You can simply try my compiled patches. Should it differ however, please carefully examine these notes and create your own SSDT patches.

7. Once you have the compiled ACPI patches, place them in `EFI/OC/ACPI/` and make sure to create matching entries within OpenCore's `config.plist`'s `ACPI/Add/` section.

/// note
The following patches are arranged alphabetically for easy cross-referencing. For the loading order, please refer to the main EFI's `config.plist`.
///

## SSDT-AC

**Load AppleACPIACAdapter**

## SSDT-ALS0

**Fake Ambient Light Sensor**
Starting with Catalina, an ambient light sensor device is required for brightness preservation. This patch fakes an ambient light sensor device `ALS0` since the x1c6 does not have one.
Why?: `ACPI0008` missing in DSDT.

## SSDT-Battery

**Enables Battery Status in macOS**
- Single battery system: only `BAT0` in ACPI, no `BAT1`.

## SSDT-DMAC

**Patch Memory Controller**
- Why?: `PNP0200` is missing in DSDT.

## SSDT-Darwin

**Detects macOS to enable other patches**

## SSDT-EC

**Alow Reads/Write and Provide an Interface with Embedded Controller via YogaSMC**
- Two parts:
  - Allow access to EC
  - Sample SSDT from YogaSMC

## SSDT-HWAC

**Fix axxess to 16byte-EC-field HWAC**

## SSDT-INIT

**Initialize System Variables**
- Disables:
  - HPET
  - DPTF
- Enables:
  - DYTC

## SSDT-Keyboard

**Remap PS2 Keys, EC Keys are handled by `BrightnessKeys.kext`**
- Remap 1: PrtSc to F13
- Remap 2: Fn + K to Deadkey
- Remap 3: Fn + P to Deadkey
- For Fn 1-12 functions, check the following option within `Preferences/Keyboard`:
  ![Fn keys](https://github.com/tylernguyen/x1c6-hackintosh/blob/main/docs/img/keyboard.png?raw=true)

## SSDT-PM

**Enables Native Intel Power Managements**
- Why?: `Processor` search in DSDT, rename `PR` to other variables as needed.

```
    Scope (\_PR)
    {
        Processor (PR00, 0x01, 0x00001810, 0x06){}
        Processor (PR01, 0x02, 0x00001810, 0x06){}
        Processor (PR02, 0x03, 0x00001810, 0x06){}
        Processor (PR03, 0x04, 0x00001810, 0x06){}
        Processor (PR04, 0x05, 0x00001810, 0x06){}
        Processor (PR05, 0x06, 0x00001810, 0x06){}
        Processor (PR06, 0x07, 0x00001810, 0x06){}
        Processor (PR07, 0x08, 0x00001810, 0x06){}
        Processor (PR08, 0x09, 0x00001810, 0x06){}
        Processor (PR09, 0x0A, 0x00001810, 0x06){}
        Processor (PR10, 0x0B, 0x00001810, 0x06){}
        Processor (PR11, 0x0C, 0x00001810, 0x06){}
        Processor (PR12, 0x0D, 0x00001810, 0x06){}
        Processor (PR13, 0x0E, 0x00001810, 0x06){}
        Processor (PR14, 0x0F, 0x00001810, 0x06){}
        Processor (PR15, 0x10, 0x00001810, 0x06){}
    }
```

## SSDT-PMCR

- Why?: `PMCR`,`APP9876` missing in DSDT.

## SSDT-PNLF

**Enables Brightness Management in macOS**
- iGPU is `PCI0.GFX0`
- Why?: `Skylake/ KabyLake/ KabyLake-R` CPU.
- Used in conjunction with `WhateverGreen.kext`.

## SSDT-PWRB

- Why?: `PNP0C0C` missing in DSDT.
- Patch power button.

## SSDT-Sleep

**Patch macOS Sleep, S3, and S0 under Windows Dual Boot**
- Comprehensive sleep/wake patch.
- Fixes restart on shutdown.
**Needs `OpenCore Patches/ Sleep.plist`**

## SSDT-TB-DSB0 to SSDT-TB-DSB6

- Patch USB 3.1
- Patch Thunderbolt 3 Hotplug
- Patch Thunderbolt 3 Power Management
- Patch Thunderbolt 3 native interfacing with macOS's System Report

## SSDT-XHC1 - USB 2.0/3.0

**Needs `OpenCore Patches/ XHC1.plist`**
- Map USB 2.0/3.0
- Patch USB Power Properties
