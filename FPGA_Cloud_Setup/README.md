### FPGA Cloud Setup
  * Compile Your Design in Local and Emulating your Design in the Cloud

<img src="https://github.com/user-attachments/assets/70aad78c-618a-4575-8ff7-78cac6f24eb3" width="800">

---
### Connecting the FPGA Hardware at Cloud

<img src="https://github.com/user-attachments/assets/65ae9ca8-3fed-42cc-9c16-1bfc8561e23c" width="800">

---
### Connecting the Device using SSH and SFTP
  * WinSCP - Free SFTP and FTP client for Windows [[Download]](https://winscp.net/eng/download.php)
  * MobaXterm Xserver with SSH, telnet, RDP, VNC and X11 [[Download]](https://mobaxterm.mobatek.net/download.html)
    
<img src="https://github.com/user-attachments/assets/473503ad-aa7f-4ae7-bfb2-e0ac2bae6273" width="800">

---
### EDA Environment Settings
* HAPS-SX Configuration Tools

```
## HAPS-SX Configuration Tools
$ /home/eda/Confpro-SX/guibin/Confpro-SX-GuiRun.sh
```
* EDA environment settings
```
## setenv.sh
## Vitis&Vivado License
export XILINXD_LICENSE_FILE=~/.Xilinx/Xil_License.lic
## AMD-Xilinx Vivado
export VIVADO_HOME=/home/Vivado/Vitis/2022.2
## AMD-Xilinx Vitis
export VITIS_HOME=/home/eda/Vitis/2022.2
## AMD-Xilinx Vitis HLS
export VITIS_HLS_HOME=/home/eda/Vitis_HLS/2022.2
```
<img src="https://github.com/user-attachments/assets/2823c35e-f82d-4dc9-bc9a-4496f9ea18c7" width="800">

---
### ZynqMP (CA53) - System Information

```
-----------------------------------------------------
$ cat /proc/cpuinfo
processor       : 0/1/2/3
BogoMIPS        : 200.00
Features        : fp asimd aes pmull sha1 sha2 crc32 cpuid
CPU implementer : 0x41
CPU architecture: 8
CPU variant     : 0x0
CPU part        : 0xd03
CPU revision    : 4
------------------------------------------------------
```
```
------------------------------------------------------
$ cat /proc/meminfo
MemTotal:       20466276 kB
MemFree:        18636132 kB
MemAvailable:   19962664 kB
------------------------------------------------------
```

```
------------------------------------------------------
$ lsmem
RANGE                                 SIZE  STATE REMOVABLE   BLOCK
0x0000000000000000-0x000000007fffffff   2G online        no    0-15
0x0000000800000000-0x000000087fffffff   2G online        no 256-271
0x0000001000000000-0x00000013ffffffff  16G online        no 512-639
------------------------------------------------------
```

```
------------------------------------------------------
$ uname -a
Linux pynq 5.15.36-xilinx-v2022.2 #1 SMP Mon Oct 3 07:50:07 UTC 2022 aarch64 aarch64 aarch64 GNU/Linux
------------------------------------------------------
```

```
------------------------------------------------------
$ cat /etc/lsb-release
DISTRIB_ID=pynqlinux
DISTRIB_RELEASE=v2.7
DISTRIB_CODENAME=Belfast
DISTRIB_DESCRIPTION="PYNQ Linux, based on Ubuntu 22.04"
------------------------------------------------------
```

```
------------------------------------------------------
$ lsusb
Bus 002 Device 001: ID 1d6b:0003 Linux Foundation 3.0 root hub
Bus 001 Device 104: ID 3185:0038 Auterion PX4 FMU v6C.x
Bus 001 Device 102: ID 046d:0825 Logitech, Inc. Webcam C270 
Bus 001 Device 003: ID ff08:9001 PUFSecurity USB HID      
Bus 001 Device 099: ID 1a40:0101 Terminus Technology Inc. Hub
Bus 001 Device 001: ID 1d6b:0002 Linux Foundation 2.0 root hub
------------------------------------------------------
```


