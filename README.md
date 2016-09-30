# osx-iso-to-usb
OSX scripts to easily burn an .iso to a usb stick.  I had a need to do
this all of the time, so I wrote this script to make the task painless.

### Usage

```bash
burn-iso-to-usb /path/to/iso /dev/diskN
```

The script will prompt you for the administrator password since it uses
dd to write to the usb stick.

You can use the `diskutil` tool to find the appropriate address for your
USB stick.  It's something like `/dev/disk5`.

The tool takes a while to run.  I'm not a `dd` expert, so I'm happy to
accept pull requests from anyone who knows how to make it run faster!
