# Nokia_N900_NITDroid
Nokia N900 NITDroid multiboot with Android 2.3 Gingerbread 

![Imgur](https://i.imgur.com/6TELxRQ.jpg?1)
![Imgur](https://i.imgur.com/fHl0ejE.jpg))
![Imgur](https://i.imgur.com/H9oOTsj.jpg)

## NITDroid Autoinstaller

a) Copy NITDroid's rootfs to /and in /home/user/MyDocs and NITDroid-Installer_0.2.8-8.deb to /home/user/MyDocs

b) Go to XTerm and launch script with:
> sh freerootfs

c) Install NITDroid automatic installer:
> dpkg -i NITDroid-Installer_0.2.8-8.deb

d) Go to main application and launch NITDroid.

e) Now reboot and enojoy the multiboot with Android 2.3 :)

## NITDroid Manual Installation

a.1) Open XTerm and type:
> root

> apt-get update

> apt-get install nitdroid-installer

OR

a.2) Copy NITDroid-Installer_0.2.8-8.deb to /home/user/MyDocs
> dpkg -i NITDroid-Installer_0.2.8-8.deb

DO NOT LAUNCH THE INSTALLER

b) Close XTerm

c) Reopen XTerm and type the following commands:

> root

> cd /home/user/MyDocs

> bzip2 -d N12_UMay.tar.bz2

> cd /home

> mkdir /and

> cd /

> mount /home /and

> cd /and

> tar xvf /home/user/MyDocs/N12_UMay.tar

> dpkg -i /home/user/MyDocs/nitdroid-installer_0.2.7_armel.deb

d) Now reboot and enojoy the multiboot with Android 2.3 :)

NOTE: If Android or multiboot don't work after reboot, try to launch the NITDroid-installer from the main application in order to fix possible issues or missing files/configuration.

# Troubleshooting

1) bzip2 command not found?
Download bzip2_1.0.5-3+0m5_armel.deb and libbz2-1.0_1.0.5-3+0m5_armel.deb. 

Place them to /home/users/MyDocs and install with:

> dpkg -i libbz2-1.0_1.0.5-3+0m5_armel.deb bzip2_1.0.5-3+0m5_armel.deb

2) Multiboot not installed correctly?
Download mtd-utils.deb, liblzo2-2.deb, i2c-tools.deb, multiboot-0.2.11.deb and backupmenu-multiboot-1.2_0.65-1.deb. 

Place them to /home/users/MyDocs and install with:

> dpkg -i mtd-utils.deb liblzo2-2.deb i2c-tools.deb
> dpkg -i multiboot-0.2.11.deb
> dpkg -i backupmenu-multiboot-1.2_0.65-1.deb
