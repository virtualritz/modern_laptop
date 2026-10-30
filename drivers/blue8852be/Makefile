# SPDX-License-Identifier: GPL-2.0
#
# Makefile for the Linux Bluetooth HCI device drivers.
#

KBUILD_MODPOST_WARN=y
KERNELRELEASE ?= $(shell uname -r)
obj-m += btusb.o btrtl.o

all:
	make -C /lib/modules/$(KERNELRELEASE)/build M=$(CURDIR) modules

install:
	make -C /lib/modules/$(KERNELRELEASE)/build M=$(CURDIR) modules_install

clean:
	make -C /lib/modules/$(KERNELRELEASE)/build M=$(CURDIR) clean
