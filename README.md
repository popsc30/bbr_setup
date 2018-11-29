https://teddysun.com/357.html
https://teddysun.com/486.html

使用root用户登录，运行以下命令：

wget --no-check-certificate -O shadowsocks-libev.sh https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks-libev.sh&&chmod +x shadowsocks-libev.sh
./shadowsocks-libev.sh 2>&1 | tee shadowsocks-libev.log
安装完成后，脚本提示如下：

Congratulations, Shadowsocks-libev server install completed!
Your Server IP        :your_server_ip
Your Server Port      :your_server_port
Your Password         :your_password
Your Encryption Method:your_encryption_method

Welcome to visit:https://teddysun.com/357.html
Enjoy it!
卸载方法：
使用 root 用户登录，运行以下命令：

./shadowsocks-libev.sh uninstall
其他事项：
客户端配置的参考链接：https://teddysun.com/339.html

安装完成后即已后台启动 Shadowsocks-libev ，运行：

/etc/init.d/shadowsocks status
可以查看进程是否启动。
本脚本安装完成后，会将 Shadowsocks-libev 加入开机自启动。

使用命令：
启动：/etc/init.d/shadowsocks start
停止：/etc/init.d/shadowsocks stop
重启：/etc/init.d/shadowsocks restart
查看状态：/etc/init.d/shadowsocks status

#检查内核
uname -r 
#谷歌的: 2.6.32-696.20.1.el6.x86_64(需修改)  搬瓦工的: 2.6.32-642.el6.x86_64

#https://moeclub.org/2017/05/10/194/
CentOS用户如遇内核不能匹配,
请参照以下示例:
使用锐速安装脚本,得知不能匹配到内核.
通过 uname -r 查看到的版本号为 2.6.32-642.el6.x86_64 ,
去查看 锐速版本库 发现有个内核版本很接近 2.6.32-573.1.1.el6.x86_64 .  (https://raw.githubusercontent.com/0oVicero0/serverSpeeder_kernel/master/serverSpeeder.txt)
执行安装命令:
wget --no-check-certificate -O appex.sh https://raw.githubusercontent.com/0oVicero0/serverSpeeder_Install/master/appex.sh && chmod +x appex.sh && bash appex.sh install '2.6.32-573.1.1.el6.x86_64'
锐速安装脚本就会强制安装内核版本为 2.6.32-573.1.1.el6.x86_64 的锐速.
安装命令中的 2.6.32-573.1.1.el6.x86_64 可自行更改.  
*centos7-bbr*
wget -N --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh && chmod +x bbr.sh && bash bbr.sh

启动锐速
如果启动成功，恭喜你!
如果启动失败，请重复 2-5 步骤! 
不要害怕失败,安装失败并不会影响系统运行.
# bbr_setup 
#锐速 
#os 	Centos 6 x86_64  
#先执行这个：

yum -y install wget

#执行完毕之后执行这个：

wget --no-check-certificate -qO /tmp/appex.sh "https://raw.githubusercontent.com/0oVicero0/serverSpeeder_Install/master/appex.sh" && bash /tmp/appex.sh 'install'

#提问 依次选择  n y y
