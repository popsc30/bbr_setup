使用root用户登录，运行以下命令：

wget --no-check-certificate -O shadowsocks-libev.sh https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks-libev.sh
chmod +x shadowsocks-libev.sh
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


# bbr_setup 
#锐速 
#os 	Centos 6 x86_64  
#先执行这个：

yum -y install wget

#执行完毕之后执行这个：

wget --no-check-certificate -qO /tmp/appex.sh "https://raw.githubusercontent.com/0oVicero0/serverSpeeder_Install/master/appex.sh" && bash /tmp/appex.sh 'install'

#提问 依次选择  n y y
