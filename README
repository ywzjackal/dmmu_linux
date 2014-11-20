#DMMU LINUX KERNEL SOURCES

##How to build
###first step
for load default am335x cpu configuration
make O=./out CROSS_COMPILE=/home/user/Software/ti-sdk-am335x-evm-07.00.00.00/linux-devkit/sysroots/i686-arago-linux/usr/bin/arm-linux-gnueabihf- ARCH=arm -C ./ tisdk_am335x-evm_defconfig
###second step
for check configuration
make O=./out CROSS_COMPILE=/home/user/Software/ti-sdk-am335x-evm-07.00.00.00/linux-devkit/sysroots/i686-arago-linux/usr/bin/arm-linux-gnueabihf- ARCH=arm -C ./ menuconfig
###third step
for build
make O=./out CROSS_COMPILE=/home/user/Software/ti-sdk-am335x-evm-07.00.00.00/linux-devkit/sysroots/i686-arago-linux/usr/bin/arm-linux-gnueabihf- ARCH=arm -C ./ uImage dtbs -j4
##How to run
kernel: ./out/arch/arm/zImage
dtb:    ./out/arch/arm/boot/dts/am335x-evm-profile2.dtb

flash kernel and dtb to nandflash, then reboot system
