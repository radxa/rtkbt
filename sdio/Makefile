SRC_DIR	:= ./bluetooth_sdio_driver
MDL_DIR	:= /lib/modules/$(shell uname -r)
DRV_DIR	:= $(MDL_DIR)/kernel/drivers/bluetooth

install:
	- rmmod btsdio
	- mv $(DRV_DIR)/btsdio.ko $(DRV_DIR)/btsdio_bak
	- rmmod btrtksdio
	make -C $(SRC_DIR)
	cp -f $(SRC_DIR)/btrtksdio.ko $(DRV_DIR)/btrtksdio.ko
	depmod -a $(shell uname -r)
	make -C $(SRC_DIR) clean
	echo "install btrtksdio success!"

uninstall:
	- mv -n $(DRV_DIR)/btsdio_bak $(DRV_DIR)/btsdio.ko
	- rmmod btrtksdio
	rm -f $(DRV_DIR)/btrtksdio.ko
	depmod -a $(shell uname -r)
	echo "uninstall btrtksdio success!"

