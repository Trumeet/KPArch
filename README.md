# GParted as an ArchISO

An ArchISO profile which contains basic Xorg server and GParted for disk maintenances.

# Known issues

Because is my first time using ArchISO, it may has some issues which I'm not sure about.

## May cannot work if

* Non-intel GPUs
* Build or run on i386 platforms

## My solution

I had build the ISO on my Dell XPS 13 9360 (x86-64 platform) and it works on the laptop and another Huawei laptop (x86-64).

# Generate ISO

Requirements:

* A running Arch Linux with network connected

## 0x00 Install ArchISO

```shell
# pacman -S archiso
```

## 0x01 Clone the repo

Clone the repo:

```shell
$ git clone https://github.com/Trumeet/GPartArch.git
```

## 0x02 Build the image

It may took about 5 minutes.

If you had built it before, delete lock files:

```shell
# rm -v work/build.make_*
```

Finally, run:

```shell
# ./archlive/build.sh -v 
```

The ISO will be saved in `out/`

# Licenses
WTFPL
