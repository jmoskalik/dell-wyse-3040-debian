# How to install Debian on DELL Wyse 3040
TESTED WITH DEBIAN 10/11/12
1. Flash `debian-XX.XX.X-amd64-netinst.iso` onto removable media and plug it into your Wyse 3040.
2. While booting the system, press F2 to enter the BIOS.
3. Change the boot device to your removable media and uncheck all other options (the default BIOS password is "Fireport").
4. Proceed with the standard installation.
5. After rebooting, boot into your Debian installation once again, but this time select "rescue mode". Follow the instructions until you see the option to "Force GRUB installation to the EFI removable media path." Click it, then click continue. Select "/dev/mmcblk0p2" in my case (you can check other mmcblk0pX options to see which one works for you), and then reboot.

## More information
https://binarypatrick.dev/posts/linux-on-dell-wyse-3040/ <br />
https://blog.roberthallam.org/2020/05/psa-dell-wyse-3040-uses-fallback-efi-location/ <br />
https://wiki.debian.org/InstallingDebianOn/Dell/Wyse%203040 <br />
