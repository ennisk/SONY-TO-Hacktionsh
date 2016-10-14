### SONY-TO-Hacktionsh

电脑型号        索尼 VAIO SVF1431AYCB 笔记本电脑  
处理器        英特尔 Core i5-4200U @ 1.60GHz 双核  
主板        索尼 VAIO ( 英特尔 Haswell-ULT )  
内存        4 GB ( 三星 DDR3L 1600MHz )  
主硬盘        东芝 MQ01ABF050 ( 500 GB / 5400 转/分 )  
显卡        NVIDIA GeForce GT 740M  ( 2 GB )  
显示器        奇美 CMN1493 ( 14 英寸 )  
光驱        松下 DVD-RAM UJ8C2 DVD刻录机  
声卡        瑞昱 High Definition Audio @ ALC233  
网卡        已更换BCM4322 完美免驱（注意换的时候要屏蔽第20针）   



### 注意点

* win: 用TranMacs把dmg镜像写入U盘
* 用 hash 里面的文件放入另一个u盘 按照

>2.1 下载最新的 Clover UEFI Loader，整理并拿出你所有需要的EFI驱动模块（driver64UEFI下的），放到一起。
把 CLOVERX64.EFI 也放到这个文件夹下。把这些文件甩到上文的存储设备里。tools 下的 EFI 应用程序也一并复制过来。
>2.2 你还需要你的 OS X 的 boot.efi；从 /System/Library/CoreServices 里获取并复制到上文的存储设备里。

来源：http://bbs.pcbeta.com/viewthread-1683114-1-1.html  

* hash 后

> 4.1 USB 启动设备
>打开你的含有 Clover UEFI Bootloader 的 USB 启动设备，到 /EFI/BOOT 里，删除原有的 BOOTX64.EFI，复制 PreLoader.efi 并改名为 BOOTX64.EFI  
>复制 CLOVERX64.EFI 到目录里并改名为 Loader.efi  
>4.2 硬盘启动设备
>It depends. 在 ESP 分区里，到 Clover 目录里，把 CLOVERX64.EFI 改名为 Loader.efi，把 PreLoader.efi 复制进来改名为 CLOVERX64.EFI  
>然后用easyuefi把clover/cloverx64.efi添加引导启动即可  


