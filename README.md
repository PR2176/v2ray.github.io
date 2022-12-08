#  前言


<a name="qy"></a>
提供v2ray与x-ui一体搭建教程，实在看不懂的，可以TG留言
<p><a href="https://t.me/wangfast" target="_blank" rel="noopener noreferrer">点击留言 </a></p> 
搭建不收费，喜欢的可以右上角点亮小星星，时间不固定，我一般半夜看TG，我看见就会回你们了，10分钟就完事儿，留言请附上vultr邮箱账号和密码。1搭建完成后请修改密码 2搭建完成后自行修改IP密码

![212333.png](https://s2.loli.net/2022/12/08/KmSArEjoGQbMF2u.png)

ssh连接后，输入命令passwd
然后输入两次新密码后，远程密码就更改成功了（一定要记清楚新修改的密码）

<!DOCTYPE html><html><head>
<body>
    <ul>
        <li><a href="#fwqzc">服务器注册</a></li>
        <li><a href="#fwqcs">节点测速</a></li>
        <li><a href="#jdht">节点后台</a></li>
        <li><a href="#ymjx">域名解析</a></li>
        <li><a href="#sshlj">SSH连接</a></li>
        <li><a href="#dajian">开始搭建</a></li>
        <li><a href="#gj">工具区域</a></li>
        <li><a href="#xhj">关于小火箭</a></li>
</body>
</html>
<a name="fwqzc"></a>
    
## 注册、购买服务器


### 第一、Vultr优点
Vultr是按小时计费，而非按月计费

IP被封可以随时更换


### 第二、登入Vultr官方网站

<p>服务器 <a href="https://www.vultr.com/?ref=9024060" target="_blank" rel="noopener noreferrer">点击注册 </a></p>


### 第三、新注册Vultr账户过程
初次登录VULTR官网的话，可能需要识别是否机器还是人类。然后我们勾选后需要两次进行图形验证。

![qwe.png](https://s2.loli.net/2022/11/17/DGftT8vHNu6WsO9.png)


设置邮箱和设置密码

![14ds.png](https://s2.loli.net/2022/11/17/XTus7BShbO1mg3w.png)

### 第四：选择充值方式激活
Vultr商家支持PayPal和支付宝等主流支付，最低10美元（大概70元，可以用两个月，用完后继续充值即可）

### 第五、流量选择

请选择开通5美元（1000G）或6美元（2000G）套餐，一般2-3人使用可以选择6美元套餐
    

    
# 现在，开始→
    
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
    
    
</br>


<a name="ymjx"></a>
##  域名解析
1.请购买国外域名，一般第一年便宜15块左右（选.xyz），国外域名续费比较贵80-90一年 https://www.namecheap.com/ 或者 https://www.godaddy.com/
    
2.注册 https://www.cloudflare.com/ （他的域名稍贵，所以在别的服务商买） ，将买的域名转到cloudflare（https://321555.xyz/domian/%E4%BB%8Enamecheap%E8%BD%AC%E7%A7%BB%E5%9F%9F%E5%90%8D%E5%88%B0cloudflare/）
    
3.也可以在namecheap解析（https://zhuanlan.zhihu.com/p/33261777）
（如果域名解析这几步你看不懂了，可能需要留言了）
    
<body>
    <ul>
        <li><a href="#qy">给我留言吧，我下班后会帮你搭建</a></li>
</body>

</br>
    
<a name="sshlj"></a>  
## ssh连接
https://jingyan.baidu.com/article/4dc40848f2c18e89d946f193.html
    
####   SSH连接工具
1<a href="https://wa6.lanzoux.com/ihjg2y3h14j/" target="_blank" rel="noopener noreferrer">FinalShell下载</a>
    
2<a href="https://wa6.lanzoux.com/iPeC7y3hryf/" target="_blank" rel="noopener noreferrer">FinalShell-MAC版下载</a>   
    
    
<a name="dajian"></a> 
###搭建（最重要） 
 
服务器连接到finalshell后
    
1.输入下面命令，然后回车
apt update -y
2.输入下面命令，然后回车
apt install -y curl   
3.输入下面命令，然后回车
apt install -y socat
4.安装脚本
curl https://get.acme.sh | sh
5.安装脚本 （将exnbdzxmnv543@gmail.com换成你自己的邮箱）   
~/.acme.sh/acme.sh --register-account -m exnbdzxmnv543@gmail.com
6.放行端口（这是三行代码，请挨个输入）
iptables -I INPUT -p tcp --dport 80 -j ACCEPT
iptables -I INPUT -p tcp --dport 443 -j ACCEPT
iptables -I INPUT -p tcp --dport 1000:65535 -j ACCEPT
7.申请证书（将baidu.com换成你的域名 ）
~/.acme.sh/acme.sh  --issue -d baidu.com   --standalone
8.申请证书（将baidu.com换成你的域名 ）
~/.acme.sh/acme.sh --installcert -d baidu.com --key-file /root/private.key --fullchain-file /root/cert.crt
9.安装xray脚本
bash <(curl -Ls https://raw.githubusercontent.com/vaxilu/x-ui/master/install.sh)
            
        

已经搭建完成了
            
后台地址你的ip:端口号（默认54321）
            
默认密码：admin/dmain或者admin/123456，会有提示  
    
    
    

<a name="gj"></a>   
## 工具区域

    
###  官方翻墙软件下载
请大家根据使用的系统下载对应的软件，主流的翻墙软件是V2ray、Clash、Shadowrocket

### Windows软件下载
    
v2rayN软件下载（Assets下v2rayN与core都下载并解压，解压后将core文件夹放到v2rayN里面就行）：v2rayN-Core.zip<a href="https://github.com/2dust/v2rayN/releases/tag/5.38">点击下载</a>
    
.NET Framework下载（windows需要4.8版本）<a href="https://dotnet.microsoft.com/zh-cn/download/dotnet-framework">点击下载</a>


v2rayN 目前需要使用微软官网 .Net 4.8 的运行库，若缺少该运行库会导致无法正常使用


#### v2rayN使用教程
    
添加节点
    
1下载完软件后，解压到桌面，无需安装，打开文件夹找到

![adsa_2.png](https://s2.loli.net/2022/10/11/pEizBmtrqWD9A1c.png)

右击选择以管理员身份运行
</br>

2复制您的节点，在服务器栏目下，找到“从剪切板导入”，左键点击即可

![324ds.webp](https://s2.loli.net/2022/10/11/YiB2TVWwkP7CndE.webp)
</br>

3导入成功后右击节点，找到“设为活动服务器”，左击即可
</br>

4上网的时候右击右下角图标，确保路由选择”绕过“，系统代理选择”自动配置“


 ![3213123fd.webp](https://s2.loli.net/2022/10/11/4gbhNBQ8lIXfG13.webp)


![fsfd123.webp](https://s2.loli.net/2022/10/11/8QdCMhfZR56qEOk.webp)
 
</br>

注意*如果显示服务一直显示启动中

![62ad632788c39.png](https://s2.loli.net/2022/10/11/vuTQrm3xgMypRaj.png)

请下载并安装 .Net Framework 4.8 后，重启电脑再打开 v2rayN，问题应该已经得到解决。   
    
    
</br>
SSR软件下载（Assets下ShadowsocksR-win.zip）：ShadowsocksR-win-4.9.2.zip<a href="https://github.com/shadowsocksrr/shadowsocksr-csharp/releases">点击下载</a>


</br>
    
### 安卓APP下载
v2Ray APP下载（Assets下v2rayNG.apk）：v2rayNG.apk<a href="https://github.com/2dust/v2rayNG/releases/tag/1.7.23">点击下载</a>
</br>
1.安装完成后，复制粘贴您的节点（也可以扫码），点击右上角“+号”，选择从剪切板导入即可

![jhhk5jh.webp](https://s2.loli.net/2022/10/11/pzMgsGDOS2N5C7h.webp)
 
</br>
 

2.点击左上角按钮，点击设置

![dasdasd5678.webp](https://s2.loli.net/2022/10/11/RONrtoBW2h6QGcp.webp)
</br>

3.域名策略：选择Match
</br>

4.预定义规则 / Predefined rules”，根据您的需求选择代理模式：

全局 / Global：代理所有流量
适用于不依赖大陆服务的用户

绕过大陆地址 / Bypassing  mainland address
适用于同时使用国内外服务的用户

 

返回到主页面，点击右下角灰色v图标，待他变绿即可
</br>
    

SSR APP下载（Assets下shadowsocksr-android.apk）：shadowsocksr-android.apk<a href="https://github.com/shadowsocksrr/shadowsocksr-android/releases">点击下载</a>


    
</br>
### MAC电脑软件下载
Clash X 软件下载（Assets下ClashX.dmg）：ClashX.dmg<a href="https://github.com/yichengchen/clashX/releases">点击下载</a>

下载的文件一般放置于用户的”下载”文件夹，使用 Finder找到下载文件。
    
MAC推荐使用ClashX


ClashX 是一个拥有 GUI界面基于Clash 可自定义规则的 macOS代理应用。

支持Shadowsocks协议和其 simple-obfs插件、v2ray-plugin 插件以及 VMess 协议和其 TCP、WebSocket 等传输方式。


#### 订阅链接配置

以一个节点为例, 给大家做个示范:

首先 双击ClashX.dmg，打开 ClashX安装程序

![ClashX-1_2.webp](https://s2.loli.net/2022/10/11/24LMOBycNHuh3wF.webp)

图：运行ClashX 安装程序

此时，桌面上会生成一个虚拟光盘，并将下载的镜像文件装载到该光盘，并弹出一个窗口，按照提示将窗口左侧的”ClashX”图标拖拽到窗口右侧的”Applications”文件夹，即完成了 ClashX 的安装。

安装过程其实就相当于把 ClashX的程序文件夹复制到 Mac电脑中，放置在”Applicationes”目录是方便应用程序的访问和使用。

 </br>

复制完成后，就可以在应用程序中看到 ClashX 应用图标，表示安装已经成功。我们就可以把虚拟光盘弹出，然后删除下载目录中的dmg文件。

第一次启动ClashX时，依次点击：打开、安装、输入密码，点击“安装帮助程序”，即可启动ClashX了（如下图）。

![daaa3d.webp](https://s2.loli.net/2022/10/11/7cEJ3rhpQCqV5k4.webp)

![Clashx-1.webp](https://s2.loli.net/2022/10/11/2oWePOfgzd8Rlba.webp)

</br>


点击菜单栏中ClashX的图标，选择 配置 => 托管配置 => 管理，

![Clashx-2.webp](https://s2.loli.net/2022/10/11/dYEAuCfXNGblS5n.webp)

然后点击 添加 ，粘贴上方 拷贝的订阅链接（注意，粘贴后如果看不到url，可能是因为多了一个空行，按一次“Backspace删除键”即可）。

![Clashx-3.webp](https://s2.loli.net/2022/10/11/aFXJQ9TenLGfBOP.webp)

![Clashx-4.webp](https://s2.loli.net/2022/10/11/4CbWDRZoqLgXPtS.webp)

</br>

点击菜单栏中 ClashX 的图标，出站模式选择 **规则**，勾选下方的 **设置为系统代理** 以及 **开机启动（可选**）。

注意，ClashX目前不支持v2ray的vless协议，所以vless节点显示为失败。

 </br>

#### 开始使用

点击菜单栏中 ClashX 的图标，然后在下方的** Proxy 策略组** 中 节点选择 选 自动选择 或者你中意的节点即可。

注意：Clash使用 HTTP HEAD方法对测试网址（server_check_url）进行网页相应测试，以确认节点的可用性。数值在5000以内均为正常值，超出则显示为超时。数值大小和网速快慢没太大关系。


### 其他注意事项

请不要修改 ~/.config/clash/config.yml 中的端口配置，否则会导致应用异常。


### ClashX 局域网代理共享

1、在 mac 终端上使用ifconfig命令获取本地IP地址。

![Clashx-5.webp](https://s2.loli.net/2022/10/11/5tsb9x8nzQ7ECL3.webp)

2、打开ClashX 控制台，在「设置」选项卡中打开「允许来自局域网的连接」，并获取 HTTP/SOCKS代理端口号。

![Clashx-6.webp](https://s2.loli.net/2022/10/11/vjigADhZlI8BESV.webp)

</br>
V2Ray软件下载（Assets下两个V2rayU按照自己电脑自行下载）：V2rayU.dmg<a href="https://github.com/yanue/V2rayU/releases">点击下载</a>

</br>
    
    
### Clash软件下载

Clash-Win版本 和 MAC版本 下载（Assets下自行选择）<a href="https://github.com/Fndroid/clash_for_windows_pkg/releases">点击下载</a>

Clash-Android版本下载（Assets下自行选择）<a href="https://github.com/Kr328/ClashForAndroid/releases">点击下载</a>

    

<a name="xhj"></a>   
 ###  关于小火箭（Shadowrocket，iOS专用）   
 
 其实iOS安装app在appstore安装即可，但是 小火箭在国区appstore已经下架了，所以只能在非国区的appstore下载安装；所以就需要非国区的appstore账号；并且小火箭也不是免费的，美国区appstore的小火箭售价是2.99美金
 </br>
一、准备工作

1.一个能接收短信的国内手机号

2.未注册过Apple ID的邮箱

3.美国地址生成器
</br>
二、注册
为方便注册，此方法全程都在手机中操作，无需电脑。

首先复制下方链接至Safari浏览器进入美国的Apple官网打开即可进入注册页面（如果打不开关闭代理）

https://appleid.apple.com/account
注册账号前需要注意三点：

1.出生日期：建议设置成大于18周岁的日期，否则会导致部分应用由于年龄限制无法使用。

2.电子邮件：建议新注册一个全新的未注册过Apple ID的邮箱。

3.手机号码：亲测，注册过国区Apple ID的手机号也可正常使用，无需纠结。

具体注册方法如下图：

![appleid1.webp](https://s2.loli.net/2022/10/11/HxehWqDMVC8rF5O.webp)

需要验证电子邮件、手机号码，依次点击下一步。

![appleid2.webp](https://s2.loli.net/2022/10/11/CbmAO53ILvwUZRS.webp)

注册成功后，会自动登录，如果没登录则重新登录刚注册的账号即可。

接下来选择付款和送货，接着再选择添加付款方式。

![appleid3.webp](https://s2.loli.net/2022/10/11/sKbiQU5Erv7u8gT.webp)

下一步填写付款方式&账单地址，这步很关键，需要借助美国地址生成器。

在生成地址前需要选择美国州，建议选以下五个免税州：

蒙大拿州（Montana）
俄勒冈州（Oregon）
阿拉斯加州（Alaska）
特拉华州（Delaware）
新罕布什尔州（New Hampshire）

美国地址生成器：>>>传送门<<<

https://www.meiguodizhi.com/
下图中标注的“由美国地址生成器生成”的内容，直接复制美国地址生成器中生成的内容即可。

![appleid4.webp](https://s2.loli.net/2022/10/11/LKG9QVFRqkdyNYT.webp)

打开App Store，点击右上角的头像，然后拉到末尾，点击退出登录。

![appleid5.webp](https://s2.loli.net/2022/10/11/UtznxTFfbjXoiYW.webp)

再次点击App Store中右上角的头像，输入前面注册的美区账号&密码，点击登录即可。

![appleid6.webp](https://s2.loli.net/2022/10/11/bGZE5XIiUh9sWyQ.webp)

然后会跳出一个弹窗，选择检查即可，接着打开同意条款与条件，选择下一页。

![appleid7.webp](https://s2.loli.net/2022/10/11/VnsUtl2JqLGIAuX.webp)

不要修改任何内容，直接点击下一页，点击继续。

![appleid8.webp](https://s2.loli.net/2022/10/11/7OWaypSkXVc3qQA.webp)

看到下图英文，点击Continue即可，美区Apple ID注册成功！

![appleid9.webp](https://s2.loli.net/2022/10/11/KTkm1Sgd9pcCBzO.webp)

此时就能下载各种美区的APP了

三、充值
部分APP需要付费的，就需要充值，有两种充值方法。

1.某宝（有封号风险）

直接搜索“苹果礼品卡”，找开店时间久，信用等级高的商家，与卖家沟通好，尽可能避免买到黑卡，若是黑卡你的账号会被封，要做好被封号的心理准备。

2.美国Apple官网购买（有门槛）

建议去苹果美国官网购买礼品卡，稳妥一些，但有门槛，需要一张双币种信用卡。

附官方购买地址：

https://www.apple.com/shop/buy-giftcard/giftcard
四、注意事项
1.不要在设置中登录美区Apple ID，以免造成不必要的麻烦！下载美区APP只需在App Store中登就行了，下载完后再换回国区账号即可。

2.如果你有在用Apple Music，切换成美区后会导致已下载的歌曲全被清空。

3.建议别把美区Apple ID当成主力账号，还是要以国区ID为主，需要下美区应用时登录就行了，以免出现意外造成不必要的麻烦。

4.付费购买的APP安装后建议别轻易卸载，即使买到黑卡账号被封，已经安装使用的APP也不影响，但卸载后账号被封就没法重新下载了。



    




