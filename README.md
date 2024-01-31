# Bottles-Offline-Installation
An installation of Bottles for those who want to install and use the program completely offline on a fresh installation of Linux. MangoHud is also included as a separate package.

The packages provided:

Bottles 51.10

This package includes soda-8.0-2, wine-8.0.2, DXVK, and VKD3D.

MangoHud 0.7.0

Please note that the installation is assuming a fresh installation of Linux with no additional flatpaks installed.

The installation was performed on a fresh installation of Linux Mint 21.2 Cinnamon x64 and was tested on three system configurations:

Intel Core 2 Duo P8400

NVIDIA GeForce 9600M GT

Intel Core i5-7300HQ

Intel HD Graphics 630

NVIDIA GeForce GTX 1050 Ti Mobile (the NVIDIA proprietary driver was not installed at the time of installation)

AMD Ryzen 5 5600H

AMD Radeon RX Vega 7

NVIDIA GeForce RTX 3060 Laptop GPU (the NVIDIA proprietary driver was not installed at the time of installation)

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

Bottles URL: https://github.com/bottlesdevs/Bottles

MangoHud URL: https://github.com/flightlessmango/MangoHud
