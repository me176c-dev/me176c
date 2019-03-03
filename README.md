<!-- SPDX-License-Identifier: CC-BY-SA-4.0 OR GFDL-1.3-or-later -->

# ASUS MeMO Pad 7 (ME176C(X))
This document gives an overview over projects for the [ASUS MeMO Pad 7 (ME176C(X))](https://www.asus.com/Tablets/ASUS_MeMO_Pad_7_ME176C/),
plus additional (general) information about the device. The issue tracker is used for issues that affect all the provided
distributions.

## Distributions
These are suggested distributions with additional instructions. You can run any Linux distribution on this tablet, although
you will need to setup more things manually for distributions not listed here.

- [Android/LineageOS](https://github.com/me176c-dev/android_device_asus_K013)
- [Arch Linux](https://wiki.archlinux.org/index.php/ASUS_MeMO_Pad_7_(ME176C(X)))
- [postmarketOS](https://wiki.postmarketos.org/wiki/Asus_MeMo_Pad_7(me176c(x)))

## Projects
These are projects you should take a look at if you want to port another Linux distribution, or help with development.

- **[me176c-boot](https://github.com/me176c-dev/me176c-boot):** Custom, unlocked bootloader with simple boot selection.  
  Suitable for both Android and Linux. Ideal for multi-boot configurations (e.g. Android and Arch Linux).
- **[linux-me176c](https://github.com/me176c-dev/linux-me176c):** Linux kernel fork with some additional patches.  
  Most of them have been upstreamed, but for example the Battery/Charging does not work with mainline.
- **[me176c-acpi](https://github.com/me176c-dev/me176c-acpi):** Patched ACPI DSDT table (part of the BIOS).  
  Necessary for some features to work properly (e.g. Touchscreen, Bluetooth, ...).

## Hardware
- **SoC:** [Intel® Atom™ Z3745](https://ark.intel.com/products/80270/) (Valleyview, Bay Trail-T), x86_64, Silvermont
- **RAM:** 1 GB :(
- **Display:** 7" 800x1280 IPS LCD
- **Internal Storage:** 16 GB
- **External Storage:** SDHCI compatible microSD card reader up to SDXC, UHS-I, DDR50 (SDR104 not supported)
- **Connectors:**
  - Micro USB 2.0 (Synopsys DWC3, XHCI for USB-OTG)
  - 2-in-1 3.5mm Audio Jack (Headphones, Microphone)
- **Touchscreen:** Goodix GT9271
- **Connectivity:** AMPAK AP6476 (WiFi + BT + GPS + FM)
  - **WiFi:** BCM43362, 802.11 b/g/n, 2.4 GHz only
  - **Bluetooth:** BCM2076B1, 4.0, BLE
  - **GPS:** [BCM4752](https://www.broadcom.com/products/wireless/gnss-gps-socs/bcm4752)
  - **FM:** Not enabled?
- **Audio:** Stereo Speakers, BYT-CR RT5640 codec
- **Battery:**
  - **Charger:** [TI BQ24192](https://www.ti.com/product/BQ24192)
  - **Fuel Gauge:** [uPI uG3105](https://www.upi-semi.com/en-article-upi-642-1611)
- **Sensors:**
  - **Accelerometer:** [Kionix KXTJ2-1009](http://kionixfs.kionix.com/en/datasheet/KXTJ2-1009%20Specifications%20Rev%209.pdf)
  - **Magnetometer:** [Asahi Kasei AK09911](https://www.akm.com/akm/en/file/datasheet/AK09911C.pdf)
  - **Hall Sensor:** "YOB8251"?
- **Camera:** Intel Atom ISP, 5 MP/2 MP, varies between ME176C and ME176CX
- **USB PHY:** [TI TUSB1211](https://www.ti.com/product/TUSB1211)
