# shScripts

#Mounts storage at ram

#! /bin/bash
mkdir /tmp/ramdisk 
chmod 777 /tmp/ramdisk
mount -t tmpfs -o size=4096M tmpfs /tmp/ramdisk/

#Unmount this storage from ram 
umount -v /tmp/ramdisk
 rm -r -f /tmp/ramdisk
