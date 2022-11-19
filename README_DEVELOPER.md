# Developer's Notes

To compile the sources by hand:

```
git clone https://github.com/blackmagic-debug/blackmagic
cd blackmagic
patch -p1 < ../blackmagic.patch
make all_platforms
```

After compiling the firmware is in the directory src/artifacts .

The patch includes:

- add separate bluepill binary
- blackpillv2: add support for processors with less ram
- for platforms with a bootloader, create an "all in one" binary of bootloader and program
