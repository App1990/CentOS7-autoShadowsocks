CentOS-7 一键安装shadowsocks

shell脚本，执行后自动搭建shadowsocks

CentOS 7使用方法：
# 安装wget组件
yum -y install wget

# 获取脚本文件
wget --no-check-certificate -O autoShadowsocks.sh https://raw.githubusercontent.com/App1990/CentOS7-autoShadowsocks/master/autoShadowsocks.sh

# 将文件标记为可执行脚本
chmod +x autoShadowsocks.sh

# 执行脚本
./autoShadowsocks.sh


# 如果执行脚本报错消息为：/bin/bash^M: bad interpreter 打开脚本设置文件格式为unix
vi ./autoShadowsocks.sh
:set ff=unix