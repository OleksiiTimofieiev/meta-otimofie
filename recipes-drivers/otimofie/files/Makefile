# obj-m := hello.o

# SRC := $(shell pwd)

# all:
# 	$(MAKE) -C $(KERNEL_SRC) M=$(SRC)

# modules_install:
# 	$(MAKE) -C $(KERNEL_SRC) M=$(SRC) modules_install


obj-m := sample_driver.o

SRC := $(shell pwd)

all:
	$(MAKE) -C $(KERNEL_SRC) M=$(SRC)

modules_install:
	$(MAKE) -C $(KERNEL_SRC) M=$(SRC) modules_install

clean:
	rm -f *.o *~ core .depend .*.cmd *.ko *.mod.c
	rm -f Module.markers Module.symvers modules.order
	rm -rf .tmp_versions Modules.symvers

# clean:
# 	$(MAKE) -C /lib/modules/$(shell uname -r)/build M=$(shell pwd) clean