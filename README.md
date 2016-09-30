"Burn" .iso images to USB disks under OSX
-----------------------------------------

OSX scripts to easily "burn" an .iso to a usb stick.  It sets the
bootable flag on the USB stick, too. I had a need to do this all
the time, so I wrote this script to make the task painless.

### Usage

```bash
burn-iso-to-usb /path/to/iso /dev/diskN
```

The script will prompt you for the administrator password since it uses
dd to write to the usb stick.  It also checks to ensure you have the
appropriate tools, and tells you if you don't.

You can use the `diskutil` tool to find the appropriate address for your
USB stick.  It's something like `/dev/disk5`.

The tool takes a while to run. For example, a 1.4GB .iso took 2.37 hours
to transfer to a generic 8 GB USB stick. YMMV based on the quality of
your USB stick.

### Contributions
I'm not a `dd` expert, so I'm happy to accept pull requests from anyone
who knows how to make it run faster, or who wants to improve
functionaltiy in general.
