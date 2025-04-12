---
icon: octicons/issue-opened-16
---

# Issues

/// warning
None of this applies to you if your machine is not an X1C6, or similar models such as the T480. You're on your own there.
///

#### Machine boots to black/BIOS, and/or selector

- Double check your EFI partition dirrectory structure. The directory structure should look as `/Volumes/EFI/EFI/`

    - `OC`
    - `BOOT`

#### Legacy macOS: Sierra, High Sierra, Catalina, and Big Sur

- These were all working on the machine at one point. They should still working with some minor tweaks to the EFI. They won't be supported by me, however. You'll have to do this yourself.

#### My X isn't working!

- Was it supposed to work? Check Summary
- Have you applied the needed patch? Check Summary, `/patches/Network Patches` and `/patches/Display Patches`.
- Is it an acknowledged, won't be fixed issue? Check [Issues/ beyond my scope](https://github.com/tylernguyen/x1c6-hackintosh/issues?q=is%3Aissue+is%3Aclosed+label%3A%22beyond+my+scope+%28for+now%29%22).

## Troubleshooting
Defer to [Dortania's General Troubleshooting](https://dortania.github.io/OpenCore-Install-Guide/troubleshooting/troubleshooting.html).

/// bug
You may find the patches under `/patches/Debug Patches/` useful in getting logs.
///
