# Bottles-Offline-Installation
An installation of Bottles for those who want to install and use the program completely offline on a fresh installation of Linux.

Please note that this installation is assuming a fresh installation of Linux with no additional flatpaks installed. MangoHud is included as a separate package.

The installation was conducted on a fresh installation of Linux Mint 21.2 Cinnamon x64 and was tested on two system configurations:

Intel Core i5-7300HQ

Intel HD Graphics 630

NVIDIA GeForce GTX 1050 Ti (NVIDIA proprietary drivers were not installed at the time of installation)



AMD Ryzen 5 5600H

AMD Radeon Vega 7 Graphics

NVIDIA GeForce RTX 3060 (NVIDIA proprietary drivers were not installed at the time of installation)



Bottles 51.10 Installation Information

The folder directories:

/home/%USERNAME%/.var/

/var/lib/flatpak/

Hidden files should be viewable. Move the ".var" folder into the "home" directory.

Open a command-line window and enter the following commands:

sudo rm -r /var/lib/flatpak/

sudo mv /home/%USERNAME%/Desktop/flatpak/ /var/lib/

The command for a "New Item" in "Edit menu":

/usr/bin/flatpak run --branch=stable --arch=x86_64 --command=bottles --file-forwarding com.usebottles.bottles @@u %u @@

The program can be launched from the "Menu".
