# QuantumultX
自用配置

[44maker自用圈x配置](https://raw.fastgit.xyz/44maker/QuantumultX/main/44makerQuantumultX.conf)
## 1️⃣大佬主页

排名不分先后（仅作自己收藏用）

-  [Orz-3](https://raw.githubusercontent.com/Orz-3/QuantumultX/master/Orz-3.conf)
-  [KOP-XIAO](https://raw.githubusercontent.com/KOP-XIAO/QuantumultX/master/QuantumultX_Profiles.conf)
-  [DivineEngine 神机](https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Outbound.conf)
-  [NobyDa野比](https://github.com/NobyDa)
-  [erdongchanyo 耳东橙](https://raw.githubusercontent.com/erdongchanyo/Rules/main/Quantumult X/LazyConf/QuantumultX_EDC-Lazy.conf)
-  **[Cuttlefish 墨鱼]([ddgksf2013/Cuttlefish: Scripts for self-use, ⛔️ fork (github.com)](https://github.com/ddgksf2013/Cuttlefish))  特别多好用的规则**
-  [limbopro 毒奶](https://raw.githubusercontent.com/limbopro/Profiles4limbo/main/full.conf)
-  [Tartarus2014 烧烤哥](https://raw.githubusercontent.com/Tartarus2014/QuantumultX-Script/main/QuanX.conf)
-  [zwf234 奇心科技](https://raw.githubusercontent.com/zwf234/rules/master/QuantumultX/qixin.conf)
-  [w37fh 北纬37度的大飛](https://raw.githubusercontent.com/w37fhy/QuantumultX/master/QuantumultX_diy.conf)
-  [blackmatrix7](https://github.com/blackmatrix7/ios_rule_script)（去广告很好用）

-  [ id77](https://github.com/id77/QuantumultX)

-  [张军]()

## 2️⃣小白配置

- [erdongchanyo 耳东橙](https://raw.githubusercontent.com/erdongchanyo/Rules/main/Quantumult X/LazyConf/QuantumultX_EDC-Lazy.conf)

  ```
  https://raw.githubusercontent.com/erdongchanyo/Rules/main/Quantumult X/LazyConf/QuantumultX_EDC-Lazy.conf
  ```

- [Cuttlefish 墨鱼](https://raw.githubusercontent.com/ddgksf2013/Cuttlefish/master/Profile/QuantumultX.conf)  特别多好用的规则

  ```
  https://raw.githubusercontent.com/ddgksf2013/Cuttlefish/master/Profile/QuantumultX.conf
  ```

## 3️⃣分流

#### 规则分流(可能有用-备忘)

- **blackmatrix7** 

  ```
  https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/QuantumultX/Advertising/Advertising.list
  ```

- **NobyDa**

  ```
  https://raw.githubusercontent.com/NobyDa/ND-AD/master/QuantumultX/AD_Block.txt
  
  https://raw.githubusercontent.com/NobyDa/ND-AD/master/QuantumultX/AD_Block_Plus.txt
  ```

## 4️⃣复写

- [奇心合集](https://raw.githubusercontent.com/zwf234/rules/master/QuantumultX/qxrules.conf)

- [墨鱼](https://raw.githubusercontent.com/ddgksf2013/Cuttlefish/master/Profile/QuantumultX.conf)

#### 获取cookie

- 野比获取cookie（爱奇艺、52破解、百度贴吧、京东、）

  ```
  https://raw.githubusercontent.com/NobyDa/Script/master/QuantumultX/yJs_Remote_Cookie.conf
  ```

- WSL33099 （内容特别全）

  ```
  https://raw.githubusercontent.com/WSL33099/QuantumultX/main/Conf/GetCookie.conf
  ```

## 5️⃣脚本

- **墨鱼脚本**

  ```
  https://github.com/ddgksf2013/Cuttlefish/raw/master/Jd/Task/jd_task.json
  ```

- **奇心脚本合集**

  ```
  https://raw.githubusercontent.com/zwf234/rules/master/QuantumultX/qixin.json	
  ```

## 6️⃣VIP解锁

- **id77**

  ```
  https://raw.githubusercontent.com/id77/QuantumultX/master/rewrite/vip.conf
  ```

- 墨鱼

  ```
  https://raw.githubusercontent.com/ddgksf2013/Cuttlefish/master/Rewrite/UnlockApp.conf
  ```

- **哔哩哔哩番剧开启1080P+ （by NobyDa）**

  ```
  #hostname=api.bilibili.com, app.bilibili.com
  
  ^https:\/\/ap(p|i)\.bilibili\.com\/((pgc\/player\/api\/playurl)|(x\/v2\/account\/myinfo\?)|(x\/v2\/account/mine\?)) url script-response-body https://raw.githubusercontent.com/zqzess/rule_for_quantumultX/master/js/backup/bilifj.js
  ```

  ```
  https:\/\/ap(p|i)\.bilibili\.com\/((pgc\/player\/api\/playurl)|(x\/v2\/account\/myinfo\?)|(x\/v2\/account/mine\?)) url script-response-body BiliHD.js
  ```

- **BiliBili 解锁1080P高码率+4K画质 (番劇和影視除外) @ddgksf2013**

  ```
  #hostname=api.bilibili.com
  
  ^https?:\/\/app\.bilibili\.com\/x\/v2\/account\/myinfo\? url script-response-body https://raw.githubusercontent.com/ddgksf2013/Cuttlefish/master/Script/bilibili_diy.js
  ```

- **#全能扫描王**

  ```
  hostname = *.intsig.net
  
  ^https:\/\/(api|api-cs)\.intsig\.net\/purchase\/cs\/query_property\? url script-response-body https://raw.githubusercontent.com/id77/QuantumultX/master/Script/camscanner.js
  ```

## 7️⃣其他

### #京东签到

- QX 1.0.10+ 脚本配置 

```
[task_local]
5 0 * * * https://raw.githubusercontent.com/NobyDa/Script/master/JD-DailyBonus/JD_DailyBonus.js, tag=京东多合一签到, img-url=https://raw.githubusercontent.com/NobyDa/mini/master/Color/jd.png,enabled=true
```

```
[rewrite_local]
#可以添加为远程重写，具体如下
# 获取京东Cookie
^https:\/\/(api\.m|me-api)\.jd\.com\/(client\.action\?functionId=signBean|user_new\/info\/GetJDUserInfoUnion\?) url script-request-header https://raw.githubusercontent.com/NobyDa/Script/master/JD-DailyBonus/JD_DailyBonus.js
# 获取钢镚签到body. 
^https:\/\/ms\.jr\.jd\.com\/gw\/generic\/hy\/h5\/m\/appSign\? url script-request-body https://raw.githubusercontent.com/NobyDa/Script/master/JD-DailyBonus/JD_DailyBonus.js
```

```
[mitm]
hostname = ms.jr.jd.com, me-api.jd.com, api.m.jd.com
```

- 获取cookie

  ①添加[远程复写]([QuantumultX/JD_Remote_Cookie.conf at master · RagBagCN/QuantumultX (github.com)](https://github.com/RagBagCN/QuantumultX/blob/master/Script/JD_Remote_Cookie.conf))

  https://raw.githubusercontent.com/RagBagCN/QuantumultX/master/Script/JD_Remote_Cookie.conf

  ②Safari浏览器打开[登录](https://home.m.jd.com/myJd/newhome.action)  https://home.m.jd.com/myJd/newhome.action 点击"我的"页面
      或者使用[旧版网址](https://bean.m.jd.com/bean/signIndex.action)  https://bean.m.jd.com/bean/signIndex.action 点击签到并且出现签到日历

- BoxJs或QX Gallery订阅地址: https://raw.githubusercontent.com/NobyDa/Script/master/NobyDa_BoxJs.json

### #网易云解锁灰色歌曲

**教程自己去找**

#### 分流

添加分流规则

```
https://raw.githubusercontent.com/GeQ1an/Rules/master/QuantumultX/Filter/Optional/Netease%20Music.list
```

#### 网易云灰色节点

```
http=music.lolico.me:39000, fast-open=false, udp-relay=false, tag= 解锁网易云节点1
http=SALVAN.ICU:19980, over-tls=false, fast-open=false, udp-relay=false, tag= 解锁网易云节点2
http=101.132.79.113:23333, fast-open=false, udp-relay=false, tag= 解锁网易云节点 3
http=MUSIC.LOLICO.ME:39000, fast-open=false, udp-relay=false, tag= 解锁网易云节点 4
http=MUSIC.GRIOUGES.CN:39000, fast-open=false, udp-relay=false, tag= 解锁网易云节点5
```

### #常用图标

- [Orz-3](https://github.com/Orz-3)/**[mini](https://github.com/Orz-3/mini)**

  🔘彩色版本 

  ```
  https://raw.githubusercontent.com/Orz-3/mini/master/Color/name.png
  ```

  🔘透明版本

  ```
  https://raw.githubusercontent.com/Orz-3/mini/master/Alpha/name.png
  ```

- [Orz-3](https://github.com/Orz-3)/**[face](https://github.com/Orz-3/face)**

  ```
  https://raw.githubusercontent.com/Orz-3/face/master/name.png
  ```

- Koolson

  ```
  img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Netease_Music.png
  
  img-url=https://raw.githubusercontent.comKoolson/Qure/master/IconSet/Telegram.png
  
  img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/WeChat.png
  
  img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/YouTube.png
  ```

  

