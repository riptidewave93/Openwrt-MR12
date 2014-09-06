Openwrt-MR12
============

Bringup Repo for the MR12 on the latest OpenWRT Nightlies


About
-----
Based on OpenWRT CHAOS CALMER r42419. May or may not work on newer revisions.

Building
--------
git sync, apply patches, menuconfig && kernel_menuconfig, build, and enjoy

Booting
-------
tftpboot 0x81000000 openwrt-ar71xx-generic-mr12-initramfs-uImage.bin; bootm

To Do
-----
* Bring up the 2nd NIC (No clue if it's an issue with the PHY, or other?)
* Bring up the Wi-Fi
* Fix Reset button GPIO
* enable sysupgrade
* Possibly more?

Notice
------
I have only tested with with TFTP booting and NOT flashing to the flash. No promises this won't break everything!
