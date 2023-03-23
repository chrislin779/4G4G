Proxidize Android: 利用Android手机创建5G/4G移动代理农场

Proxidize Android Legacy是一款Android应用程序，可以让任何人使用他们的Android手机创建4G或5G移动代理农场，而不需要任何其他设备。只需下载该应用程序，点击连接，您的移动代理就会自动生成。

Proxidize创建了Proxidize Android作为Proxidize MPM（移动代理制造商）的概念验证。该应用程序达到了其目的，但由于以下原因最终从Google Play商店下架。

Proxidize Android Legacy是即将推出的Proxidize Portable应用程序的前身，后者将是该应用程序的重大改进。

在其他语言中阅读此页面： [русский](https://github.com/proxidize/proxidize-android/blob/main/README.ru.md)

![Overview](https://i.imgur.com/gsRoRBt.png)

<div align="center"> </br><a href="https://github.com/proxidize/proxidize-android/releases/download/v2.1.4/Proxidize.Android.Legacy.v2.1.4.apk">
    <img src="https://i.imgur.com/HkPj7Fx.png" height="auto"/>
  </a>
</br></br></br></div>

</div>


## What Is Proxidize:

Proxidize是由一组工程师发起的跨国合作，旨在实现对Web数据和自动化的民主化访问。阅读Proxidize宣言：https://proxidize.com/manifesto/


<div align="center"> <a href="https://proxidize.com/">
    <img src="https://i.imgur.com/3FEWrk5.png" height="auto"/>
  </a>
</div>

<div align="center">
  <h2>Proxidize</h2>
  <a href="#how-to-create-a-5g-or-4g-mobile-proxy-on-android-phones-turn-your-phone-into-a-mobile-proxy">Start Making Mobile Proxies</a>
  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
  <a href="#rotationchanging-the-ip-how-to-change-mobile-proxy-android-ip-address-using-airplane-mode">IP Rotation</a>
  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
  <a href="https://proxidize.com/">Website</a>
  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
  <a href="https://proxidize.com/android">Docs</a>
  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
  <a href="https://proxidize.com/blog">Blog</a>
  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
  <a href="https://twitter.com/proxidizehq">Twitter</a>
  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
  <a href="#proxidize-portable">Proxidize Portable</a>
  <br />
  <hr />
</div>

---

Proxidize Android Legacy的特点

![image](https://user-images.githubusercontent.com/107770894/190168239-2084da54-9b5a-4ed6-9ab8-3bd21671adf5.png)


    在Android、MacOS或Windows设备上创建移动或住宅的HTTP(S)或SOCKS5代理。
    可手动使用按钮旋转/更改IP，也可使用特定旋转间隔自动更改IP。
    提供用作链接/URL的旋转/更改IP的API。
    在使用应用程序生成移动代理时连接到移动数据。
    在使用应用程序生成住宅代理时连接到Wi-Fi。
    由全球服务器管理的超快速负载平衡。
    添加自定义的隧道服务器以获得更高的安全性和速度。
    实验性功能：更改操作系统指纹以提高运营安全性。
    实验性功能：将连接分离到Wi-Fi后端以获得更好的速度。



---

工作原理和架构

Proxidize Android Legacy通过通过反向代理与隧道服务器建立连接，然后启动本地HTTP代理服务器来工作。这使得代理可以从Web的任何地方访问，因为隧道服务器处理了端口转发和路由。

<div align="center">
    <img src="https://i.imgur.com/9UAAcx3.png" height="auto"/>
</div>


该应用程序将在10000到60000之间选择一个随机端口，使用该端口连接到客户端，然后基于该随机端口以及随机生成的用户名和密码创建代理服务器。


---

    Proxidize Android - 在Android手机上创建5G/4G移动代理
        什么是Proxidize？
        Proxidize Android Legacy的功能
        如何工作及架构
        Proxidize Android Legacy vs Proxidize Mobile Proxy Maker
        如何在Android手机上创建5G/4G移动代理：（将手机变成移动代理）
            在Windows MacOS上使用（在WindowsMacOS上创建5G或4G移动代理）
        使用代理
        轮换/更改IP地址（如何使用飞行模式更改移动代理Android IP地址）
            自动更改IP地址
            手动更改IP
            通过URL / API更改IP
        支持的Android版本和设备
        部署您自己的服务器
            示例
        不连接隧道服务器即可使用该应用程序
        报告问题
            您应该报告的问题类型
            如何报告问题
            任何与应用程序无关的问题都将被关闭，例如
        更新
        常见问题解答：
            为什么谷歌标记此应用程序为有害应用程序/恶意软件？
            我的代理无法使用，显示“代理拒绝连接”错误？
            我的代理以前可以使用，但现在停止工作了，能帮忙解决吗？
            为什么我的代理很慢？
            此应用程序在哪些地方可用？
            [我一直收到“407错误”或代理一直要求验证？](#


---

Proxidize Android Legacy与Proxidize Mobile Proxy Maker相比不是一种替代品，而是一个概念验证。你可以在小规模的个人项目中使用这个应用程序，但一旦需要商业级解决方案，你将需要Proxidize MPM，原因如下：

    这样的应用程序由于底层基础架构主要设计用于物联网设备而不是代理，所以天然不可靠。
    速度较慢。由于入站和出站连接都通过同一网络接口进行传输，因此你得到的速度将是移动速度的五分之一。
    难以进行大规模管理。从Proxidize设置一个20个调制解调器套件只需要10分钟，但设置20个手机将需要整整一天，如果不是更长时间。

---

如何在安卓手机上创建5G或4G移动代理：（将您的手机变成移动代理）

<div align="center">
    <img src="https://i.imgur.com/ASSDAe2.png" height="auto"/>
</div>


    下载Proxidize Android Legacy APK文件。
    安装APK文件到您的设备。
    打开应用程序并点击“连接”。
    复制代理，您可以在任何地方使用它。

现在，您已经创建了自己的5G/4G移动代理！

以下是在Windows或macOS上使用Proxidize Android Legacy创建5G或4G移动代理的步骤：

    下载任何Android模拟器，如BlueStacks。
    在模拟器内部下载Proxidize Android Legacy APK文件（从模拟器打开此页面并下载APK）。
    安装APK文件到模拟器中。
    打开应用并按“连接”按钮。
    复制代理并在任何地方使用它。

---

## Using the Proxy

Format:
```
IP:Port:Username:Password
```

Example:
```
1.1.1.1:1565:abc:xyz
```

Explained:
```
IP or Hostanme: 1.1.1.1
Port: 1565
Userrname: abc
Password: xyz
```
---
## Rotation/Changing the IP (How to Change Mobile Proxy Android IP Address Using Airplane Mode)

Proxidize Android Legacy has built-in rotation. To set it up, you need to set the app as the default assistant in your settings.


### Automatically Changing the IP Address:

<div align="center">
    <img src="https://i.gyazo.com/8c923c64c2996452c78993003e023d94.png" height="auto"/>
</div>

Proxidize Android Legacy allows you to set a rotation/IP change interval. To use it, you need to:
- Press "AUTO CHANGE IP" button on the home page.
- Select the rotation interval you wish to use.
- Select a time in minutes. Anything less than 30 minutes will harm your phone.
- Press "SET" and your settings will be applied.



### Changing the IP Manually:

<div align="center">
    <img src="https://i.gyazo.com/ad6fa87d163262908253e99cf2f436ab.png" height="auto"/>
</div>


To change the IP address manually, you simple need to press the change IP button.



### Changing the IP via URL/API:

<div align="center">
    <img src="https://i.gyazo.com/ded5e4abaf6f19ca75ff5045889dced4.png" height="auto"/>
</div>

Proxidize Android Legacy generates an IP change link/URL/API that you can use anywhere to change the IP.

To change the IP using the rotation link, you need to:
- Copy the change IP URL under "IP Change Link/API" by pressing the "COPY" button.
- Use the link anywhere or send a GET request to it.

A success response is:

```{"response":"success"}```


---
## Supported Android Versions & Devices

Proxidize Android Legacy supports all ```armeabi-v7a``` running ```Android 6.0``` to ```Android 12```

Supported Android API from ```API 23``` to ```API 31```.

Tested devices:

```
All Android 6.0+ phones
Samsung A Series
Samsung S Series
Samsung M Series
Samsung Note Series
Google Pixel
OnePlus
```
---

## 部署您自己的服务器

<div align="center">
    <img src="https://i.gyazo.com/cc24b11d87379469f06ac8f15257dcbe.png" height="auto"/>
</div>

Proxidize Android Legacy允许您部署自己的隧道服务器，避免使用共享/拥挤的服务器。要做到这一点，您需要：

    在任何主机上创建一个新服务器。确保您在公共网络上，所有端口都是公开可访问的。
    编辑配置文件以添加您的服务器信息。
    编辑“CUSTOM SERVER”字段以添加您的新服务器。

示例：

    服务器IP = 5.5.5.5

    确保服务器为x86-64或AMD64，运行Ubuntu 20.04

    SSH进入您的服务器

ssh username@5.5.5.5

    克隆此存储库

git clone https://github.com/proxidize/proxidize-android.git

    进入存储库目录

cd ./proxidize-android

    编辑server.ini文件以添加身份验证令牌

vi或nano ./server/server.ini

    添加以下信息，用您自己的值替换PORT和TOKEN。除非您有更改它的理由，否则保持端口值为2000。
    
    [common]
bind_port = PORT
authentication_method=token
token = TOKEN

TOKEN用于验证哪些客户端被允许连接到此服务器。它可以是任何随机字符集，例如12345678。

 给权利
chmod +x server/server

    启动服务器

setsid ./server/server -c ./server/server.ini &

setsid用于在关闭终端后保持进程运行。

    通过转到菜单>更改服务器>自定义，将新服务器信息添加到应用程序中。

HOST = 新服务器的公共IP地址。在本示例中，它是5.5.5.5。

Binding Port = 您选择的端口。

Token = 您选择的令牌。

    保存详细信息，退出应用程序，然后再次打开它并连接即可连接到您的新隧道服务器。

---

## Reporting Issues

### Types of Issues That You Should Report:

- App keeps crashing on a specific device/Android version.
- Bypass battery optimization not working on a specific device/Android version.
- App stops working after a while on any
- Proxy Refusing Connection web error, even though the port and host are correct.
- If you see any of the following errors: 12020, 12033, or 12165.

### How to Report the Issue:

- Full description of the issue including screenshots and any error codes
- Full device manufacturer & model name. E.g. Samsung SM-A105L
- Include a screenshot of the "Software information" page
- Full instructions to replicate the issue.


### Any Issues Unrelated to the App Will Be Closed, Such As::

- I sent 1,000 threads to scrape Amazon and now the IP is banned.
- I'm using vanilla puppeteer or Chrome and I keep getting blocked or my proxy is detected.
- Any form of 407/authentication error. This means you're not using the right credentials. Refer to format section.
- 502 or 504 if you're using rotation. This happens when you're connecting in the middle of a rotation.
- Any situation where you're using your own server. (Unless you can replicate the issue when using the default servers as well.)


---
## Updates:

This app is no longer maintained by Proxidize, but I (Abed) will be working on it in my free time.

Edit: I ended up finishing most of the planned features before schedule. So chances are I won't be making any updates to this app for a while.

Things I'll be adding:

- [x] Supporting Android 12
- [x] Add Android wake lock to keep the proxy alive.
- [x] Custom server from application.
- [x] Save ports between sessions.
- [x] In-app IP rotation button.
- [x] Automated IP rotation.
- [x] IP rotation API
- [x] Supporting more devices such as Asus, Alcatel, etc.
- [x] Auto-detect nearest tunneling server.
- [x] SOCKS proxies.
- [x] Prevent duplicate ports on server.
- [ ] Showing the public IP on the app interface.
- [ ] Change proxy format.

If you're updating to v2.0.0 from v1.0.0 make sure to delete v1.0.0 first.

---


## FAQ:

### Why is the app marked as harmful app/malware by Google?

A few months after publishing the app, Google marked it as harmful/PUP/malware app. I suspect it's because there's some Google watchdog that sniffed the traffic and found something harmful that was being transmitted by some of the users. Or it's possible that the behavior of the traffic being unencrypted and routed to a single server was similar to typical harmful app behavior that come across Google in the Play Store.

There are also a few AVs that have marked the tunneling client fast revers proxy, as a PUP, and it's possible Google Play Store did the same.

I've made some mitigations against this by changing the binaries to change the hash, but I suspect Google will still mark it as harmful by reading the strings, so you will need to disable Play Protect, otherwise, the app will likely get automatically deleted.

### My proxy isn't working with ```Proxy Refusing Connection``` error?

Make sure you're using the correct port value, then exit the app and start it again. There's a very small chance you used an already used port.

### My proxy stopped working after it used to work, can you help?

Exit the app and start it again. If it still doesn't work, make sure the app is still running on your device. Then please tweet [@Proxidizehq](https://twitter.com/proxidizehq) and we'll take a look.

### Why is my proxy slow?

The app uses reverse proxies created via websockets route to forwarding facing proxies. This technology is slow, unreliable and there's nothing I can do about it with the limited time that I have to work on this project. Apps based on this specific tunneling technology were created for simple IoT use cases, and not for pushing full bandwidth or proxies.

The Proxidize team is working on an entirely new app called **Proxidize Portable**, which will address all the short comings of this app using proprietary technology.

Another thing is such apps send both incoming and outgoing traffic from the same device, which means you will always get half the speed that you would normally get when testing the speed directly on your phone. If speed is important, you should use the full Proxidize MPM-OP: https://proxidize.com/

### Where will this app work?

This app will work everywhere, unless:
- You are in countries that have ISP-level firewalls that block any proxied connections via DPI.
- You are behind a corporate firewall that blocks unknown ports.

### I keep getting a ```407 Error``` or the proxy keeps asking for authentication?

Make sure you're not mixing the small ```l``` with a capital ```I```.


---

## Proxidize Portable

We are currently working on a new application called "Proxidize MPM-Cloud Portable" or Proxidize Portable for short. The new app will address all the deficiencies of this one and will have the following features:

1. 5-10x higher speeds than Proxidize Android Legacy
2. Custom OS Fingerprint
3. Send & Receive SMS via interface/API
4. Manage all devices from web interface
5. Manage unlimited phones via grouping, categories and more.
6. Use any server from dozens of countries.
7. Custom DNS
8. Get 99.99% uptime
9. Dual-stacking IPV4/IPV6 support
10. Load-balancing between multiple phones.
11. Setting multi-phone IP rotation/load balancing pools.
12. And much more!

