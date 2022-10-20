ArchLinux-PS4 drivers

## How i install the drivers ?
If you want to install the drivers using the precompiled files just use ```sudo pacman -U``` in the 'Compiled/' folder for each files.

If you want to compile and install the drivers just use ```makepkg -si``` in for each folder inside and this will install the drivers.

## If you want to compile for PS4pro follow these steps:

Edit the PKGBUILD file on mesa-ps4
On line 31 rename "mesa.patch" to "mesa-ps4pro.patch" without the quotes and save the changes.
On line 89 rename "patch -p1 -i ../mesa.patch" to "patch -p1 -i ../mesa-ps4pro.patch" without the quotes and save the changes.

Edit the PKGBUILD file on lib32-mesa-ps4
On line 33 rename "mesa.patch" to "mesa-ps4pro.patch" without the quotes and save the changes.
on line 86 rename "patch -p1 -i ../mesa.patch" to "patch -p1 -i ../mesa-ps4pro.patch" without the quotes and save the changes.

Then compile and install the drivers just use ```makepkg -si``` in for each folder inside and this will install the drivers.
