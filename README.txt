
本固件（非Lite版） 自带 负载均衡/MWAN3分流助手/IPTV助手，但他们都是默认关闭的，如果你需要启用他们，需要到 “系统”--“启动项”里找到。
他们分别是
负责均衡 -- mwan3
MWAN3分流助手 -- mwan3helper
IPTV助手 -- iptvhelper
将其改成已启用，然后重启系统。

支持网页上传刷机和网络自检

命令行刷机
wget ROM下载地址 -O /tmp/rom.zip
unzip rom.zip
sh /root/flash_rom.sh /tmp/rom具体取名.img.gz /dev/mmcblk0 gz

刷机工具：http://www.ksite.xyz/contents/balena-etcher.html

刷机后初始化时段请耐心等待。

正确的重启网络的姿势：定时重拨--马上执行--等待。路由器能上网，你也能上路由器，那说明你手机等设备可能需要关网重连，或者多等等也行。

设置宽带拨号：https://jingyan.baidu.com/article/3ea514891e5b8613e71bba79.html

关闭IPV6：https://jingyan.baidu.com/article/0eb457e573e2e842f0a90567.html （反过来就是打开）。不需要ipv6的还可以把WAN6接口删除（这有时很重要）

更新和安装DDNS姿势：网页端--系统--软件包--更新列表--输入ddns--安装luci-app-ddns--到一些ipk网盘找到ddns-scripts_aliyun等使用文件传输上传并装上(使用DDNS时你可能需要关闭flowoffload 或 sfe -- 如果有开启)

docker也一样，通过官方源来获取最新的软件包。

某些usb-wifi芯片也一样可通过软件包安装

*刷机并首次完成配置后建议你重启路由一次（重启姿势：网页端-系统-重启-点击执行）*

分流地址：

 https://www.90pan.com/o134832（密码：ksite）

 https://pan.baidu.com/s/12-BFGJKtCih6CtuL0V3NDQ (提取码: 32kq)
 
 一些ipk：https://kongfl888.lanzous.com/b04sj203c （密码:abw4）
 
 (不定期更新)
 
 [K]2020!
 