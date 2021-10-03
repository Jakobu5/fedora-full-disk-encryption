# Full Disk Encryption

To enable full disk encryption on Fedora Workstation 31, first we backup the content of the boot partiton.
Then the boot partition will be reused as a LUKS1 encrypted partition.
After the unlock of the LUKS boot partition GRUB (the boot loader) is reconfigured by adding the *cryptodisk* module to the configuration `/etc/default/grub`.
Then the config can be recreated. 
