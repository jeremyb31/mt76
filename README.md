#mt76
cd mt76
make -C /lib/modules/$(uname -r)/build M=$(pwd) modules
sudo cp mt76x02-lib.ko /lib/modules/5.4.0-58-generic/kernel/drivers/net/wireless/mediatek/mt76/
make -C /lib/modules/$(uname -r)/build M=$(pwd) clean

