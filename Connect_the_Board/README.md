### Opening a USB Serial Terminal

* Connect the micro-USB cable from your computer to the board and open a terminal. 
  * You can use the terminal to check the network connection of the board. You will need to have terminal emulator software installed on your computer. 
  * [PuTTY](https://www.putty.org/) and [MobaXterm](https://mobaxterm.mobatek.net/) are applications that can be used, and is available for free on Windows. 

* To open a terminal, you will need to know the COM port for the board.
Full terminal Settings:

```
115200 baud, 8 data bits, 1 stop bit, No Parity, No Flow Control
```

```
$ sudo chmod 666 /dev/ttyUSB*
$ sudo putty -serial -sercfg 115200,8,n,1,N -fn "client:Ubuntu Mono 16"  /dev/ttyUSB1 &
```

---
### SSH/SFTP/SCP

* SSH/SFTP/SCP: SSH allows secure file transfer using [SCP and SFTP](https://help.ubuntu.com/community/SSH/TransferFiles)
  * WinSCP - Free SFTP and FTP client for Windows [[Download]](https://winscp.net/eng/download.php)

* Download MobaXterm Xserver with SSH, telnet, RDP, VNC and X11 [[Download]](https://mobaxterm.mobatek.net/download.html)
  * From this console window, you will be allowed to run the Unix commands you need: ls, cd, grep, awk, tail, cut, sed, wget, All the essential Unix tools are present.

<img src="https://github.com/user-attachments/assets/3a422987-7f05-41eb-a243-39b4dbccbaec" width="800">
