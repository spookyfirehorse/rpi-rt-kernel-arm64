# rpi-rt-kernel-arm64


rt-kernel very simple
https://forums.raspberrypi.com/viewtopic.php?t=381025

##download

wget https://forums.raspberrypi.com/download/file.php?id=74529

do not edit config.txt auto initramfs is enabled kernel load automatic
       sudo apt build-dep linux  -y 

       sudo ./build-kernel -b default -c 7 -j 6 -u -d        ### rpi5 rt-kernel
       sudo ./build-kernel --branch rpi-6.18.y -c 7 -j 6 -u -d 


       sudo ./build-kernel -b default -c 6 -j 6 -u -d        ### rpi4 rt-kernel
       sudo ./build-kernel --branch rpi-6.18.y -c 6 -j 6 -u -d 


       
      sudo mkinitramfs -o "/boot/initrd.img-$(uname -r) $(uname -r)"
