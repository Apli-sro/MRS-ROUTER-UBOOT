UBOOT MOD FOR MRS-ROUTER based on RT5350F-OLinuXino
GPIO18:
low: uboot - silent start - enable WD od GPIO0
hi: uboot console & web update firmware



RT5350 linux SDK from Ralink modified to open webpage on ethernet port
=======
Webpage can be triggered by gpio 0 (default) or gpio 27 (use setenv webgpio 27 in console)

DO NOT BUILD WITH GCC > 3.5.2 !!!

Suitable tool chain is available in Uboot/toolchain

For VoCore run make menuconfig in Uboot directory, set path to toolchain, chip type to ASIC,
chip ID to rt5350 and DRAM Component to 256 Mb

Credits:

Wolfgang Denk and all the others that work on Das U-boot, even though this project is based on a pre-historic version of u-boot their work is incredible.

Stevenylai and Ralink who are responsible for the GitHub project this is forked from.

Pepe2k whose webfailsafe for AR93xx routers was plagarized shamelessly in my work.

Manfeel whose blog gave me very helpful hints about byte order. I wish I had found this much earlier in my work since I duplicated much of his other work the hard way.
http://blog.csdn.net/manfeel/article/details/13096075

Vonger who gave us the VoCore

I take responsibility for the kludgy, ugly code you may find here, but it does work.
