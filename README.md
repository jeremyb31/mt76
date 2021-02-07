This is no longer needed as the fix was released in Ubuntu kernel 5.4.0-65

#mt76

cd mt76

make -C /lib/modules/$(uname -r)/build M=$(pwd) modules

sudo cp mt76x02-lib.ko /lib/modules/$(uname -r)/kernel/drivers/net/wireless/mediatek/mt76/

make -C /lib/modules/$(uname -r)/build M=$(pwd) clean

