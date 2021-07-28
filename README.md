# gentoo_files
Contains gentoo linux files and kernel configs

Get gentoo linux zen kernel from here : https://github.com/zen-kernel/zen-kernel/releases/
or 

Get Linux-ck by emerge -aq ck-sources 

#### Complete Overhaul Required ####

mount -o rw,noatime,ssd,compress=zstd,space_cache,subvol=@ /dev/nvme0n1p6 /mnt



mount -o rw,noatime /dev/nvme0n1p5 /mnt/boot/efi/
mount -t proc proc /mnt/proc/
mount -t sysfs sys /mnt/sys/
mount -o bind /dev /mnt/dev
mount -t devpts pts /mnt/dev/pts
chroot /mnt /bin/bash


