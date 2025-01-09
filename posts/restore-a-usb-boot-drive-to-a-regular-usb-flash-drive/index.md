# U 盘启动盘恢复为普通 U 盘


近使用 U 盘安装系统，制作系统启动盘。安装完系统后，发现 U 盘中 EFI 分区，需要把它删掉。

* 首先使用快捷键 Win&#43;R，输入 cmd 打开命令提示符；
* 然后输入 diskpart；
* 输入之后会显示磁盘列表，通常电脑的磁盘为 0，U 盘为 1；
* 接下来输入 sel disk 1；
* 最后输入 clean，U 盘恢复为普通 U 盘了。


---

> 作者:   
> URL: https://blog.wenyi.org/posts/restore-a-usb-boot-drive-to-a-regular-usb-flash-drive/  

