# efibootmgr_bootnext
Quick bash script that sets the UEFI BootNext variable using a case insensitive grep and efibootmgr 

Took 2 minutes to make, but nice to keep around in case it ever gets deleted

### How to Use
Put it in your /usr/local/bin maybe or your favorite path folder.
Write "bootnext arch" or "bootnext windows" or whatever and it will be updated.
Write "bootnext windows now" to also have it sudo reboot immediately.

### Quick Summary

 1. efibootmgr prints summary and we case insensitive grep it for whatever the first user arg is (no spaces or use quotes)
 2. If there is a result from this grep, we pull out the boot number and the name of the entry
 3. We use efibootmgr -n to set the next OS to boot and print a little message
 4. Else, we print a failure message
