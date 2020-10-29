# Plymouth

Change theme in Ubuntu 20.04.
## Installation

Download the folder and copy to /usr/share/plymouth/themes.

```bash
cp -r new_plymouth_folder /usr/share/plymouth/themes
```

Install the new Plymouth theme as the default theme using the command below.

```bash

sudo update-alternatives --install
/usr/share/plymouth/themes/default.plymouth default.plymouth
/usr/share/plymouth/themes/new_plymouth_folder/new_plymouth.plymouth 100

```

Change the default theme to yours by entering the theme number.

```bash
sudo update-initramfs -u
```

For the changes take effect run the following command.

```bash
sudo update-initramfs -u
```


