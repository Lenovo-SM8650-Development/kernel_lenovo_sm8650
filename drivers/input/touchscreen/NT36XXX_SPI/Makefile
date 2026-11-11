#
# Makefile for the Novatek NT36xxx touchscreen driver.
#

# Each configuration option enables a list of files.
ifeq ($(CONFIG_ARCH_KIRBY),y)
EXTRA_CFLAGS += -DBUILD_KIRBY_TOUCH
else ifeq ($(CONFIG_ARCH_LAPIS),y)
EXTRA_CFLAGS += -DBUILD_LAPIS_TOUCH
endif

obj-$(CONFIG_TOUCHSCREEN_NT36XXX_SPI) += nvt_36xxx.o
nvt_36xxx-y +=  nt36xxx.o
nvt_36xxx-y +=  nt36xxx_fw_update.o
nvt_36xxx-y +=  nt36xxx_ext_proc.o
nvt_36xxx-y +=  nt36xxx_mp_ctrlram.o
nvt_36xxx-y +=  nt36xxx_platform.o
