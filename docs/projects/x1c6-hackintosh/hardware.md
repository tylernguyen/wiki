---
icon: material/harddisk-remove
---

# Hardware Prep

## Storage

/// bug
The factory PM981 NVMe drive does not play well with macOS.

Replace it with an aftermarket NVMe for easily installation and better macOS compatibility.
///

For installation on the factory drive `PM981`, please refer to [Issue #43](https://github.com/tylernguyen/x1c6-hackintosh/issues/43). I do, however, recommend against this.

See [dortania/Anti-Hackintosh-Buyers-Guide :octicons-arrow-up-right-16:](https://dortania.github.io/Anti-Hackintosh-Buyers-Guide/Storage.html) for up-to-date storage recommendations.

/// tip
You can install an additional M.2 2242 NVMe drive in the WWAN card slot.

This is particularly useful if you intend to dual-boot Windows/Linux. However, the drive will only run at PCIe x1 speed.
///

## WiFi and Bluetooth

/// tip
If your laptop did not come with WWAN, you can purchase additional antennas to add to your laptop. This is useful when using WiFi/Bluetooth cards that have 3 antennas.
///

The laptop's default wireless card can be patched to function under macOS.

The BCM94360CS2, along with a M.2 NGFF adapter will work natively under macOS.

The two options, however, can be limited in speed and compatibility. I recommend upgrading to a newer Intel card for more modern WiFi and Bluetooth standards.

See [![OpenIntelWireless](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/OpenIntelWireless.png){ .twemoji }  OpenIntelWireless | Compatibility :octicons-arrow-up-right-16:](https://openintelwireless.github.io/itlwm/Compat.html) for Intel cards compatibilities.

## CPU Cooler

/// info
[:simple-reddit:{ .reddit } Reddit :octicons-arrow-up-right-16:](https://www.reddit.com/r/thinkpad/comments/c7zpah/x1_carbon_6th_gen_horrible_cooling_fan_design/): The X1C6 has different CPU cooler manufacturers, and they differ greatly in noise and performance.

Replacement CPU coolers can be found on eBay.
///

I also advise to redo the stock thermal application.

- [Grizzly Kryonaut](https://www.thermal-grizzly.com/en/products/16-kryonaut-en) is often recommended. You may also look into other brands such as Noctua or Arctic.
- [Grizzly Conductonaut](https://www.thermal-grizzly.com/produkte/25-conductonaut) (liquid metal) gives better thermal performance, given that you are experienced and inclined with the application.

[:simple-youtube:{ .youtube } @der8auer](https://www.youtube.com/@der8auer) shown himself tuning this exact machine model with liquid metal:

1. [:simple-youtube:{ .youtube } Lenovo X1 Carbon G6 - Liquid Metal and Tuning (Part 1)](https://www.youtube.com/watch?v=FXR5-HwIre8)
2. [:simple-youtube:{ .youtube } Lenovo X1 Carbon G6 - Liquid Metal and Tuning (Part 2)](https://www.youtube.com/watch?v=1yimz_Wy0lM)

## Battery Replacement

![Replacement Battery Cell](https://assets.tylernguyen.wiki/projects/x1c6-hackintosh/Battery-cell.png){ align=right width=300 }

Depending on the battery health (cycle count, max capacity), consider getting a replacement battery cell. Genuine battery cells are the Lenovo Part 01AV430 and Lenovo Part 01AV431.

Avoid eBay sellers, especially from overseas. Look to purchase from the Lenovo Parts Store or from trust worthy vendors such as iFixit.

/// tip
The X1 Carbon 5th and 6th Generation uses the same battery cell.
///
