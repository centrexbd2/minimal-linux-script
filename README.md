# Minimal Linux Script

One script which generates fully functional live Linux ISO image with minimal effort. This is based on the first published version of [Minimal Linux Live](http://github.com/ivandavidov/minimal) with some improvements taken from the next releases. All empty lines and comments have been removed and the script has been modified to reduce the overall length.

The script below uses **Linux kernel 6.7.1**, **BusyBox 1.36.1** and **Syslinux 6.03**. The source bundles are downloaded and compiled automatically. If you are using [Ubuntu](http://ubuntu.com) or [Linux Mint](http://linuxmint.com), you should be able to resolve all build dependencies by executing the following command:

```bash
sudo apt install wget make gawk gcc bc bison flex xorriso libelf-dev libssl-dev
```

After that simply run the below script. It doesn't require root privileges. In the end you should have a bootable ISO image named `minimal_linux_live.iso` in the same directory where you executed the script.

```bash
./minimal.sh
```

Note that this script produces very small live Linux OS with working shell only and no network support. The network functionality has been implemented properly in the [Minimal Linux Live](http://github.com/ivandavidov/minimal) project which is extensively documented and more feature rich, yet still produces very small live Linux ISO image.
