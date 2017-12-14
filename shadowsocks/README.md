# koolshare.github.io
####For koolshare.cn 小宝merlin改版固件 软件中心

<b>shadowsocks文件夹下的内容，用于向路由器内shadowsocks功能推送更新</b><br/>
<b>此项目仅用于merlin koolshare ARM架构改版固件</b><br/>

* <b>shadowsocks.tar.gz</b><br/>
此文件为shadowsocks文件夹的打包，通过路由器访问 [https://raw.githubusercontent.com/koolshare/koolshare.github.io/master/shadowsocks/shadowsocks.tar.gz](https://raw.githubusercontent.com/koolshare/koolshare.github.io/master/shadowsocks/shadowsocks.tar.gz) 获取安装包更新。

## 如果你更新出现问题，请按照以下方式手动更新：
<pre>
cd /tmp
wget --no-check-certificate --timeout=15 https://raw.githubusercontent.com/koolshare/koolshare.github.io/master/shadowsocks/shadowsocks.tar.gz
tar -zxvf /tmp/shadowsocks.tar.gz
chmod +x /tmp/shadowsocks/install.sh
sh /tmp/shadowsocks/install.sh
</pre>

## 如果你需要更新历史版本，这里以 1.5.0版本为例：(需要更新其它版本，只需要自行更改版本号，所有历史版本存档目录：https://github.com/koolshare/koolshare.github.io/tree/acelan_softcenter_ui/shadowsocks/history)

<pre>
cd /tmp
wget --no-check-certificate https://raw.githubusercontent.com/koolshare/koolshare.github.io/acelan_softcenter_ui/shadowsocks/history/shadowsocks_1.5.0.tar.gz
tar -zxvf /tmp/shadowsocks.tar.gz
chmod +x /tmp/shadowsocks/install.sh
sh /tmp/shadowsocks/install.sh
</pre>

* <b>history文件夹</b><br/>
该文件夹用于存放shadowsocks历史安装包，需要回滚历史版本的，可以下载对应版本，然后手动安装。

* <b>version</b><br/>
在线版本号和shadowsocks.tar.gz的md5校验值，用于判断更新。