# Actions-OpenWrt

使用 SSH远程 GitHub Actions 云编译Openwrt固件

### NanoPi R2S 固件链接地址（https://github.com/DHDAXCW/R2S-2021）

### 默认编译

- 用户名：root 密码：password 管理IP：192.168.2.1
- 已开启SSH，可自定义选择编译，自动生成`.config`

## 使用方法

-   增加了SSH远程编译，通过 tmate 连接到 GitHub Ac­tions 虚拟服务器环境，可直接进行 make menuconfig 操作生成编译配置，或者任意的客制化操作。也就是说，你不需要再自己搭建编译环境了。
  这可能改变之前所有使用 GitHub Ac­tions 的编译 Open­Wrt 方式。复制 SSH 连接命令粘贴到终端内执行，或者复制链接在浏览器中打开使用网页终端。（网页终端可能会遇到黑屏的情况，按 Ctrl+C 即可）

cd openwrt && make menuconfig
 
 完成后按Ctrl+D组合键或执行exit命令退出，后续编译工作将自动进行。
 
### 提示

在你的存储库介绍中添加一些你构建的固件的元信息（比如固件体系结构和安装的软件包），这样可以节省其他人的时间。

### 注意！
- 只能给r4s固件ssh远程配置，其他不能。😓
### ssh1 x86最新固件

- 最新版本 跟r4s源码相似，但是插件完全跟r4s一样

### Lean OpenWrt.yml r4s最新固件

- 爽就好了嘿嘿

### 版本日志 1.18号

-  待机超10天无法上网,需要重启才解决（已修复）

- 再次增强DHCP稳定性，增加多种协议（已优化） 

- 优化DNS在加载情况下无法启动进后台（已增强） 

- 降级到DDNS版本，最新版有问题（已降级，不清楚没试过） 

- 再次添poeee拔号多种协议（后期提高拔号稳定） 

- 优化部分内核代码重新优化一下 

- 更新rk3399驱动（友善官网提供） 

- 更新网卡驱动 

- 修复了其他小问题

## 版本日志 1.29号

- 增新了ipv6客户端，快速获取ipv6

- 修复了adguardhome插件无法启动问题，改为Lienol源码仓库的插件

## 后续更新
