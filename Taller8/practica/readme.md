## Taller 8 Embebidos

`sudo mknod /dev/memory32 c 50 0`

`make -C /usr/src/linux-headers-$(uname -r) M=$(pwd modules)`

`sudo chmod 666 /dev/memory32`

`sudo insmod memory_32.ko`

`echo -n H > /dev/memory32`

`cat /dev/memory32`

`sudo rmmod memory_32`