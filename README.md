## 简介

本一键脚本在萌咖大佬的脚本基础上开发，实现了懒人式一键网络重装 Debian / Ubuntu / CentOS 系统及dd方式安装系统。解决了云服务商提供模板镜像体积过大、预装软件过多、不够纯净等问题。（用到了 @Vicer 萌咖大佬的脚本，感谢~）

项目地址：https://github.com/shendaiqilin/Shell

**支持重装的系统：**

* Debian 9/10
* Ubuntu 18.04/16.04
* CentOS 6/7
* 自定义DD镜像

**特性/优化：**

* 自动获取IP地址、网关、子网掩码
* 自动判断网络环境，选择国内/外镜像，再也不用担心卡半天了
* 超级懒人一键化，无需复杂的命令
* 解决萌咖脚本中一些导致安装错误的问题
* CentOS 7 镜像抛弃LVM，回归ext4，减少不稳定因素
## 使用方法：

```
wget --no-check-certificate -O AutoReinstall.sh https://git.io/AutoReinstall.sh && bash AutoReinstall.sh
```

## 注意事项

* 重装后系统密码为：Pwd@Linux，安装后请尽快修改密码，Linux系统建议启用密钥登陆。
* OpenVZ / LXC 架构系统不适用
* 不适于甲骨文/ikoula等平台主机
