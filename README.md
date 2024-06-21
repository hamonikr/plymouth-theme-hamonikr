# plymouth-theme-hamonikr

plymouth theme for HamoniKR OS

## This package contains three types of themes.

1) hamonikr-dark.plymouth black with logo
![screenshot](./app.gif)

2) hamonikr-default.plymouth : colorful with logo
![screenshot2](./app2.gif)

3) bgrt-hamonikr.plymouth : Display oem logo only (bgrt)

# Install

## Ubuntu, Debian, LinuxMint

```
wget -qO- https://pkg.hamonikr.org/add-hamonikr.apt | sudo -E bash -

sudo apt install plymouth-theme-hamonikr

```

After installing the package, the basic theme is type 3, which only displays the logo of the manufacturer.

How to change to another theme is:
```
sudo update-alternatives --config default.plymouth


There are 5 choices for the alternative default.plymouth (providing /usr/share/plymouth/themes/default.plymouth).

  Selection    Path                                                                   Priority   Status
------------------------------------------------------------
  0            /usr/share/plymouth/themes/hamonikr-default/hamonikr-default.plymouth   600       auto mode
* 1            /usr/share/plymouth/themes/bgrt-hamonikr/bgrt-hamonikr.plymouth         400       manual mode
  2            /usr/share/plymouth/themes/bgrt/bgrt.plymouth                           110       manual mode
  3            /usr/share/plymouth/themes/hamonikr-default/hamonikr-default.plymouth   600       manual mode
  4            /usr/share/plymouth/themes/hamonikr-dark./hamonikr-dark..plymouth       500       manual mode
  5            /usr/share/plymouth/themes/spinner/spinner.plymouth                     70        manual mode

Press <enter> to keep the current choice[*], or type selection number: 

```
Enter the desired theme number here.

Now run in the terminal as follows to apply the theme.

```
sudo update-grub

OR

sudo update-initramfs -k all -u
```
