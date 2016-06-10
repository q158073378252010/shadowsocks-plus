# shadowsocks-plus
-----
发布页面: https://www.ifxor.com/archives/297/
基于 Shadowsocks Go 版本，加入了以下特性：

- 启动后降低权限至 nobody , 增强安全性。
- 与 kcptun 集成，配合相应客户端可加速传输。
- 网页控制面板

支持系统： Debian/Ubuntu (32/64位)，CentOS (32位，64位需自行安装32位C和C++支持库)

一键安装：
rm ssplus_install.sh ; wget --no-check-certificate https://www.ifxor.com/installers/ssplus/ssplus_install.sh && bash ssplus_install.sh

运行：ssplus-server -c /etc/ssplus.conf

开机自启动：将以上命令加入 /etc/rc.local 即可。

默认端口：6719

默认密码：SSplus_Default_Password

加密算法：chacha20

kcptun 加速端口为SS端口号 + 10000，即默认为 16719

SS端口号范围 1000 – 9999。

配置文件：/etc/ssplus.conf（格式和原版一样）
