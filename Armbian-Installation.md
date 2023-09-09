# Before following these steps...
## MAKE SURE YOU KNOW WHAT YOU'RE DOING. I WILL NOT TAKE ANY RESPONSIBILITY FOR BROKEN/BRICKED DEVICES!

# What is this all about?
### This tutorial describes the installation of Armbian OS in the Tanix TX9 TV Box, but most of these steps can be generalized and applied to other chinese TV boxes. If you own a different model, you can find information about your specific requirements with just a bit of research in forums.
### PS: This tutorial was written in September 8th, 2023. The steps may differ as newer versions of Armbian are released.

# Index

* [Requirements](#requirements)
* [Gathering info](#gathering-info)
* [Downloading and flashing image](#downloading-and-flashing-image)
* [Editing the contents of SD card](#editing-the-contents-of-sd-card)
* [Booting](#booting)

# Requirements

- SD Card (minimum 8Gb, preferably larger and fast)
- A computer
- A keyboard
- A mouse (optional)
- A toothpick (yeah...)

# Gathering info

Open PlayStore in the TV box and install AIDA64. Open the app, and in the `System` tab, look for the `Device` section. Take note of the model shown there; in my case, it was the `p281` SoC, which means my board is the S905W model.
Still in the same tab, take note of the `Total Memory` and `Internal Storage Total Space` sections.

# Downloading and flashing image

Go to the Armbian archive related to your board model ([this one's for S9XX](https://armbian.site-meganet.com/dl/aml-s9xx-box/archive/)) and download the latest version of the OS. There are many files with similar names; the ones actually containing the image are those ending with `.img.xz` (you can also opt for `.img.xz.torrent`).

After the file is downloaded, extract the image from the .xz file using a tool such as unxz for Linux, or WinRar for Windows. Once that's done, plug your SD card and flash the image on it using a flashing tool (Balena Etcher is a good option, available on both OSes). *Be sure to backup any important data before flashing, as it will be overwritten!*.
PS: If you're on Windows, the system might alert that your SD card is corrupted after the flashing is done. You can ignore this message.

# Editing the contents of SD card

