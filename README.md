# Mi-Router-4C
Install Openwrt

cd /tmp

curl https://github.com/AchmadPR/Mi-Router-4C/blob/main/openwrt-21.02.0-ramips-mt76x8-xiaomi_mi-router-4c-squashfs-sysupgrade.bin --output firmware.bin 

./busybox sha256sum firmware.bin

mtd -e OS1 -r write firmware.bin OS1
