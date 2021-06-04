# archfi

Just a simple bash script wizard to install Arch Linux after you have booted on the official Arch Linux install media.

With this script, you can install Arch Linux with two simple terminal commands.

This wizard is made to install minimum packages (Base, bootloader and optionally archdi).

At the end of this wizard, you can install or launch [archdi](https://github.com/MatMoul/archdi) (Arch Linux Desktop Install) to install and configure desktop packages.

You can watch my videos to see how to use it [here](https://www.youtube.com/playlist?list=PLytHgIKLV1caHlCrcTSkm5OF2WSVI1_Sq).

## How to use

First, boot with the [last Arch Linux image](https://www.archlinux.org/download/) with a [bootable device](https://wiki.archlinux.org/index.php/USB_flash_installation_media).

Then make sure you have Internet connection on the Arch iso. If you have a wireless connection the [`iwctl`](https://wiki.archlinux.org/index.php/Iwd#iwctl) command might be useful to you. You can also read the [Network configuration](https://wiki.archlinux.org/index.php/Network_configuration) from the Arch Linux guide for more detailed instructions.

Then download the script with from the command line:

    curl -LO archfi.sf.net/archfi

If SourceForge is down, use this instead:

    curl -LO matmoul.github.io/archfi

Finally, launch the script:

    sh archfi

Then follow the on-screen instructions to completion.

If you require extra help, visit the provided video playlist and follow my example.

## More custom install

    sh archfi -cpl {URL of your custom package list}

You can find a sample custom package list file in the samples folder.

## For developers

You can test your script with this command :

    sh archfi -t {githubusername} {branchname}

Example :

    sh archfi -t matmoul master
