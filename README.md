# Realtek RTL8125 NIC driver for ESXi 6.7

This source code is based on realtek official source, VMware-ESXI-67U3-ODP and VMware-TOOLS-10.2.0-ODP.

Just do these steps:
- Prepare the building environment, I did it on CentOS 7
- Log in with root, make a folder name 'build' on /, make folder toolchain and vsphere in /build.
- Copy and extract gcc-4.8.0, binutils-2.22, glibc-2.3.4-2.41 to /build/toolchain/src 
- Compile the toolchain, dest path is /build/toolchain/lin64
- Extract and copy vmkdrivers-gpl from 67U3-ODP to /build/vsphere
- Copy build-r8125.sh to /build/vsphere/vmkdrivers-gpl/
- Copy r8125 folder to /build/vsphere/vmkdrivers-gpl/vmkdrivers/src_9/drivers/net
- Run build-r8125.sh


适用于 ESXi 6.7 的 Realtek RTL8125 网卡驱动程序
本源码基于realtek官方源码，VMware-ESXI-67U3-ODP和VMware-TOOLS-10.2.0-ODP。

只需执行以下步骤：

- 准备搭建环境，我是在CentOS 7上做的
- 使用root登录，在/上创建一个文件夹名称'build'，在/build中创建文件夹toolchain和vsphere。
- 将gcc-4.8.0、binutils-2.22、glibc-2.3.4-2.41复制解压到/build/toolchain/src
- 编译toolchain，目的路径为/build/toolchain/lin64
- 将 vmkdrivers-gpl 从 67U3-ODP 提取并复制到 /build/vsphere
- 将 build-r8125.sh 复制到 /build/vsphere/vmkdrivers-gpl/
- 将 r8125 文件夹复制到 /build/vsphere/vmkdrivers-gpl/vmkdrivers/src_9/drivers/net
- 运行 build-r8125.sh
