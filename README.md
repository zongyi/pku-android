## 模拟器下载
* [windows](http://lab.zynotes.com/android-sdk_r24.4.1-windows.zip)
* [linux](http://lab.zynotes.com/android-sdk_r24.4.1-linux.tgz)
* [macosx](http://lab.zynotes.com/android-sdk_r24.4.1-macosx.zip)

* [三个img文件](http://lab.zynotes.com/img.tar)

## 模拟器运行
模拟器执行需要4个参数：
1. 运行目录
2. system image
3. ramdisk image
4. user data image
5. kernel

以x86为例，命令为：
``` bash
emulator-x86 -sysdir out/ -system out/system.img -ramdisk out/ramdisk.img -data out/userdata.img -kernel out/kernel-qemu
```

## 方法说明
* 此方法可以避免装双系统，只要将虚拟机中编译出的内核拷贝出来，再用模拟器执行即可
* 此外，这个方法不需要下载aosp，只需要内核部分代码
