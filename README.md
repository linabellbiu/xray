# div xray && 科学上网 && VLESS协议 && XTLS

# 脚本摘录大神[@hijkpw](https://github.com/hijkpw)[一键搭建脚本](https://github.com/hijkpw/scripts/tree/master) 非常感谢为自由上网做出的贡献

[Xray一键脚本](https://github.com/wangxudong123/xray/blob/main/xray.sh)

#### 前期准备:
1. 有基本linux技巧
2. 准备一台SSH能连接到境外的VPS，可参考https://my.vultr.com/
3. 需要有域名(可参考[域名服务商https://www.namesilo.com/](https://www.namesilo.com/))dns解析到当前境外服务器的ip
4. 需要ssl证书[从阿里获取免费证书](https://itlanyan.com/get-free-ssl-certificates-from-aliyun/)


#### 配置xray服务端
1. [Xray一键脚本](https://github.com/wangxudong123/xray/blob/main/xray.sh) 放到服务器的/root 目录下
2. 把ssl证书([从阿里获取免费证书](https://itlanyan.com/get-free-ssl-certificates-from-aliyun/))放到服务器的/root 目录下
3. 执行脚本，会看到下面的界面
  ```
  [root@vultr ~]# ./xray.sh 
  #############################################################
  #                     Xray一键安装脚本                      #
  # 作者: 网络跳越(hijk)                                      #
  # 网址: https://hijk.art                                    #
  # 论坛: https://hijk.club                                   #
  # TG群: https://t.me/hijkclub                               #
  # Youtube频道: https://youtube.com/channel/UCYTB--VsObzepVJtc9yvUxQ #
  #############################################################
    1.   安装Xray-VMESS
    2.   安装Xray-VMESS+mKCP
    3.   安装Xray-VMESS+TCP+TLS
    4.   安装Xray-VMESS+WS+TLS(推荐)
    5.   安装Xray-VLESS+mKCP
    6.   安装Xray-VLESS+TCP+TLS
    7.   安装Xray-VLESS+WS+TLS(可过cdn)
    8.   安装Xray-VLESS+TCP+XTLS(推荐)
    9.   安装trojan(推荐)
    10.  安装trojan+XTLS(推荐)
   -------------
    11.  更新Xray
    12.  卸载Xray
   -------------
    13.  启动Xray
    14.  重启Xray
    15.  停止Xray
   -------------
    16.  查看Xray配置
    17.  查看Xray日志
   -------------
    0.   退出
   当前状态：未安装

    请选择操作[0-17]：  
    
   ```
 4. 输入 8
 5. 看提示操作，一般都是默认就好。等待安装完成后会重启服务器 
 6. 配置xray客户端:[V2rayN 配置教程以及配置VLESS协议](https://v2xtls.org/v2rayn-4-12%e9%85%8d%e7%bd%ae%e6%95%99%e7%a8%8b/)
    > V2rayN：3.28版本起支持xray，只需要下载Xray-core，将解压的文件放到V2rayN-Core文件夹下即可。需要注意的是V2rayN 4.0版本移除了PAC，改用路由规则.

相关文章
- [xray教程](https://itlanyan.com/xray-tutorial/)
- [V2rayN 配置教程以及配置VLESS协议](https://v2xtls.org/v2rayn-4-12%e9%85%8d%e7%bd%ae%e6%95%99%e7%a8%8b/)
- [V2Ray高级技巧：流量伪装](https://itlanyan.com/v2ray-traffic-mask/#bnp_i_2)
  > 亲测不怎么好用，各种问题
- [V2Ray客户端](https://itlanyan.com/v2ray-clients-download/)
- [Xray 的客户端](https://www.jamesdailylife.com/xray_software)
- [好用的vps vultr](https://my.vultr.com/)
  > 按照小时收费。被墙还可以删除重新选择实例和ip
- [域名服务商https://www.namesilo.com/](https://www.namesilo.com/)
  > 便宜，但是解析dns超级慢可能需要2个小时
- [从阿里获取免费证书](https://itlanyan.com/get-free-ssl-certificates-from-aliyun/)
