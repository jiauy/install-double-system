# install-double-system
安装windows linux双系统
#### 背景：更换NVME固态硬盘后之前的PE进不去了，记录此次过程
- 安装老毛桃最新版U盘启动工具，可以支持NVME
- 进入PE，对NVME固态硬盘快速分区，GUID格式。分两个区，一个用来安装windows,一个用来装linux
- 在PE中启动windows 10安装程序后等待安装完成，期间会有重启
- windows安装成功后进入系统，windows+X打开磁盘管理，将NVME预留给linux的分区删除，变为未设置
- 使用USBwriter.exe 将linux系统写入到U盘当中，并重启
- U盘启动，安装linux系统
