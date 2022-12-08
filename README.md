#  前言

提供v2ray与x-ui一体搭建教程，实在看不懂的，可以TG留言（https://t.me/wangfast） ， 帮忙搭建不收费，右上角点亮小星星，10分钟完事儿，时间不固定，我一般半夜看TG，我看见就会回你们了，请附上IP地址


![123.png](https://s2.loli.net/2022/12/08/rzfMEwc1lKU6CyW.png)


搭建完成后自行修改密码

![212333.png](https://s2.loli.net/2022/12/08/KmSArEjoGQbMF2u.png)

ssh连接后，输入命令passwd
输入两次新密码后，远程密码就更改成功了（一定要记清楚新修改的密码）

<!DOCTYPE html><html><head>
<body>
    <ul>
        <li><a href="#fwqcs">节点测速</a></li>
        <li><a href="#jdht">节点后台</a></li>
        <li><a href="#fwqzc">服务器注册</a></li>
        <li><a href="#ymjx">域名解析</a></li>
        <li><a href="#sshlj">SSH连接</a></li>
        <li><a href="#dajian">开始搭建</a></li>
        <li><a href="#gj">工具区域</a></li>
   
</body>
</html>

# 现在，开始
<a name="fwqcs"></a>    
## 关于测速

很多朋友让我们把速度测速放上来，这个没什么参考性，跟网络、设备及地区有关系，家庭普通100-200M带宽看个2K、4K/,完全没有问题（我看YouTube一般在8w-15w kbps），8K需要你的显卡及显示屏支持，不然会显得一卡一卡的，不流畅

节点速度跟宽度运营商（现在一般都是光纤入户）、区域、家庭带宽有关系（想要达到最佳效果，得配上千M网卡（现在电脑一般自带）、网线（推荐山泽6类线，2块钱1米），千兆路由器）

普通网线及路由器，速度已经够用了


## YouTube 4K视频*3840x2160



### 家庭宽带200M（普通网线）

![家庭宽带200M（普通网线）](https://cdn.shopify.com/s/files/1/0658/7357/6188/files/mryc-0908_2048x2048.png?v=1662608583)

### 家庭宽带200M（六类网线）

![家庭宽带200M（六类网线）](https://cdn.shopify.com/s/files/1/0658/7357/6188/files/mzyc-200M_2048x2048.png?v=1662611318)

家庭宽带越高，速度也会越快


### cloudflare下载测速

![cloudflare测速](https://cdn.shopify.com/s/files/1/0658/7357/6188/files/mzcscloudflare_2048x2048.png?v=1662618129)

### speedtest.cn下载测速
![speedtest.cn下载测速](https://cdn.shopify.com/s/files/1/0658/7357/6188/files/adada56w_2048x2048.png?v=1662937362)

大家可以自行测速：不同地区进行下载的速度（建议在全局代理的环境下测试，并尽量关闭后台占用网络资源较多的程序，以提高测试结果的准确性）


#### [测速点一](http://cordcloud.speedtestcustom.com/)



#### [测速点二](http://aaaaaa.speedtestcustom.com/)


#### [测速点三](http://rixcloud.speedtestcustom.com/)


#### [测速点四](https://speed.cloudflare.com/)
    

    
<a name="jdht"></a>
## 节点后台功能    
###### 1.可自行为其他用户添加各类客户端节点



###### 2.可自行设置其他用户可使用流量



###### 3.可自行设置其他用户到期时间    
<img src="https://s2.loli.net/2022/11/26/mrB6bFvEc7WNdtl.png" alt="系统状态">
<img src="https://s2.loli.net/2022/11/26/qfDE4WAxyUNbnrm.png" alt="入站列表">
<img src="https://s2.loli.net/2022/11/26/5bkeTdEwxXUMuIy.png" alt="添加节点">
<img src="https://s2.loli.net/2022/11/26/znfpyY6ORb2lmMx.png" alt="面板设置">
<img src="https://s2.loli.net/2022/11/26/c9DjT8o6yALM7Jl.png" alt="用户设置">
<img src="https://s2.loli.net/2022/11/26/nsRhjECgXeNl1WF.png" alt="xray设置">  
    
#### vmess设置

![vmess](https://s2.loli.net/2022/10/11/l2EFQaq6wAObXBo.webp)



#### vless、Trojan等其他协议可自行设置
    

域名：就是你的域名，如baidu.com（无www），要是我帮忙搭建的，会提供给你免费的域名

路径：

公钥文件路径
/root/cert.crt

密钥文件路径
/root/private.key   
    
    
<a name="fwqzc"></a>
### 注册流程


### 第一、Vultr优点
Vultr是按小时计费，而非按月计费

IP被封可以随时更换


### 第二、登入Vultr官方网站

<p>服务器 <a href="https://www.vultr.com/?ref=9024060" target="_blank" rel="noopener noreferrer">点击注册 </a>.</p>


### 第三、新注册Vultr账户过程
初次登录VULTR官网的话，可能需要识别是否机器还是人类。然后我们勾选后需要两次进行图形验证。

![qwe.png](https://s2.loli.net/2022/11/17/DGftT8vHNu6WsO9.png)


设置邮箱和设置密码

![14ds.png](https://s2.loli.net/2022/11/17/XTus7BShbO1mg3w.png)

### 第四：选择充值方式激活
Vultr商家支持PayPal和支付宝等主流支付，最低10美元（大概70元）

### 第五、流量选择

请选择开通5美元（1000G）或6美元（2000G）套餐，一般2-3人使用可以选择6美元套餐



## 工具区域

####   SSH连接 
    <a href="https://wa6.lanzoux.com/ihjg2y3h14j/" target="_blank" rel="noopener noreferrer">FinalShell下载</a>
    <a href="https://wa6.lanzoux.com/iPeC7y3hryf/" target="_blank" rel="noopener noreferrer">FinalShell-MAC版下载</a>
 
    
#####  官方翻墙软件下载
请大家根据使用的系统下载对应的软件，主流的翻墙软件是V2ray、Clash、Shadowrocket

Windows软件下载
v2rayN软件下载（Assets下v2rayN与core都下载并解压，解压后将core文件夹放到v2rayN里面就行）：v2rayN-Core.zip<a href="https://github.com/2dust/v2rayN/releases/tag/5.38">点击下载</a>

SSR软件下载（Assets下ShadowsocksR-win.zip）：ShadowsocksR-win-4.9.2.zip<a href="https://github.com/shadowsocksrr/shadowsocksr-csharp/releases">点击下载</a>


安卓APP下载
v2Ray APP下载（Assets下v2rayNG.apk）：v2rayNG.apk<a href="https://github.com/2dust/v2rayNG/releases/tag/1.7.23">点击下载</a>

SSR APP下载（Assets下shadowsocksr-android.apk）：shadowsocksr-android.apk<a href="https://github.com/shadowsocksrr/shadowsocksr-android/releases">点击下载</a>


MAC电脑软件下载
Clash X 软件下载（Assets下ClashX.dmg）：ClashX.dmg<a href="https://github.com/yichengchen/clashX/releases">点击下载</a>

V2Ray软件下载（Assets下两个V2rayU按照自己电脑自行下载）：V2rayU.dmg<a href="https://github.com/yanue/V2rayU/releases">点击下载</a>


Clash软件下载
Clash-Win版本 和 MAC版本 下载（Assets下自行选择）<a href="https://github.com/Fndroid/clash_for_windows_pkg/releases">点击下载</a>

Clash-Android版本下载（Assets下自行选择）<a href="https://github.com/Kr328/ClashForAndroid/releases">点击下载</a>


*下载软件时，打开网页找到Assets位置，可以看到下载文件


    




