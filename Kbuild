obj-$(CONFIG_RTKBT_SDIO) 	+= btrtksdio.o
btrtksdio-y := sdio/bluetooth_sdio_driver/btrtk_sdio.o \
			   sdio/bluetooth_sdio_driver/btrtl.o \
			   sdio/bluetooth_sdio_driver/rtk_coex.o

obj-$(CONFIG_RTKBT_UART)        += rtk_hci_uart.o
rtk_hci_uart-y := uart/bluetooth_uart_driver/hci_h4.o \
                           uart/bluetooth_sdio_driver/hci_ldisc.o \
                           uart/bluetooth_sdio_driver/hci_rtk_h5.o \
                           uart/bluetooth_sdio_driver/rtk_coex.o

obj-$(CONFIG_RTKBT_USB) 	+= rtk_btusb.o
rtk_btusb-y := usb/bluetooth_usb_driver/rtk_coex.o \
			   usb/bluetooth_usb_driver/rtk_misc.o \
			   usb/bluetooth_usb_driver/rtk_bt.o
