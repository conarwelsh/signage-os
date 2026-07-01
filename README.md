# signage-os

Releases for the sous.tools signage OS

## How to inject your specific WiFi/SSH credentials right now:
- Keep the SD Card Plugged In: After the flash finishes, your computer will likely unmount and then remount a small FAT32 partition from the SD card called boot or bootfs.
- Enable SSH: Just create a completely blank, empty file named exactly ssh (no file extension) in the root of that boot drive. This tells the OS to force-enable the SSH daemon immediately on startup.
- Add WiFi: In that same boot folder, you can create a wpa_supplicant.conf file (if it is based on standard Raspberry Pi OS) or edit the network settings in the injected user-data file to include your local network credentials.
