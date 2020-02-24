# 搬瓦工搭建 SSR
1.打开搬瓦工主页，点击「Services」,选择「My Services」。

![](pic/01.png)

2.可以看到您所购买的服务器，点击「KiwiVM Control Panel」。

![](pic/02.png)

3.点击左侧「Install new OS」。

![](pic/03.png)

4.选择「debian-8-x86_64」，勾选我同意，点击「Reload」。

![](pic/04.png)

5.记住密码和端口号。

![](pic/05.png)

6.点击左上角「Admin functions」。

![](pic/06.png)

7.可以看到显示 Running，表示成功。

![](pic/07.png)

8.Mac 打开终端，输入以下字符，按回车键。
```
ssh root@110.110.110.110 -p 11111
```
>注：110.110.110.110修改为您搬瓦工 ip，11111 修改为刚才记下的端口。

![](pic/08.png)

9.输入您刚才记下的密码，按回车键。

![](pic/09.png)

10.复制下面代码粘贴，按回车键。
```
wget --no-check-certificate -O shadowsocks-all.sh https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks-all.sh
```

![](pic/010.png)

11.复制下面代码粘贴，按回车键。
```
chmod +x shadowsocks-all.sh
```

![](pic/011.png)

12.复制下面代码粘贴，按回车键。
```
./shadowsocks-all.sh 2>&1 | tee shadowsocks-all.log
```

![](pic/012.png)

13.输入 `2` ，按回车键。

![](pic/013.png)

14.输入密码，按回车键。
>密码自定义

![](pic/014.png)

15.输入端口，按回车键。
>端口号范围在 1-65535 之间

![](pic/015.png)

16.输入 `2`，按回车键。

![](pic/016.png)

17.按回车键。

![](pic/017.png)

18.按回车键。

![](pic/018.png)

19.按回车键。

![](pic/019.png)

20.等待代码走完（约 3-5 分钟），您将看到搭建好的路线信息，请保存下来即可。