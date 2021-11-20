# 重要更新
* 2021年10月28日，更新了F大最新的打包方式，具体为`固件打包输出路径从tmp改成output了,这样就允许用tmpfs挂载到tmp而不占用太多内存(得自己挂，当系统内存大于4GB时可行，mount -t tmpfs  none  /opt/openwrt_packit/tmp），提高打包速度，减少出错概率。`

* 2021年10月3日，固件升级方式发生一些变化，升级文件改为openwrt-update-amlogic，首先进入目录`cd /mnt/mmcblk2p4` 下载后`chmod +x openwrt-update-amlogic`,之后把固件下载到同一个目录后,执行`./openwrt-update-amlogic`有提示输入`y`为保留配置升级，选`n`相当于重装。升级完成后系统会自动重启，稍安勿躁。

* 2021年6月18日，上游大雕全面更新了最新代码，受影响，60+或60+o版本升级61版本的，建议重新安装，如果不想刷U盘全新安装，也可以用升级脚本升级，只是选择是否保存配置时，选“n”

* 2021年6月6日，加入科学上网常用ipk输出Releases


* 2021年5月24日，同步更新F大佬的快照功能
![增加快照功能](https://cdn.jsdelivr.net/gh/hublj/fx-n1/img/op.jpg)

使用方法：固件新刷入或采用新版的 update-xxx-openwrt.sh 脚本升级之后就具备了快照功能，工具包名称：由于取名困难，故采用了 flippy 为命令名称（/usr/sbin/flippy)，在ssh或ttyd下输入即可，全程中文菜单，全交互式操作。

# 特别提醒
不要盲目追新，仓库自动打包的固件或插件，均为最新的版本，最新版本意味着有BUG；如果之前固件使用稳定，无需追新。
总结一句话：**追新有风险、更新须谨慎**

# +和+o的版本区别
+的内核版本较新；+o的版本相对+的内核更稳定；f大不太建议N1等盒子使用+的版本，因此比较推荐使用+o的版本。


# 默认IP及密码
默认IP 192.168.1.201  密码 password




# 感激
 * [flippy](https://www.right.com.cn/forum/space-uid-285101.html)
 * [coolsnowwolf/Lede](https://github.com/coolsnowwolf/lede)
 * [mingxiaoyu](https://github.com/mingxiaoyu)
 * [hibuddies](https://github.com/hibuddies/openwrt/)
