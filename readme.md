# 这是一个没做完的洛谷CMD客户端 #


###
### 登录终于做好了！
### 我选择曲线救国的方式（分明就是懒
### 目前的方式是在洛谷主页登录后拿到Cookie，输入cookie以登录
### 详细教程见login-chrome.md
### 目前登录可以做到这一步了：~~（洛谷第三方客户端的长足进步~~
### *是手动隐藏，到时候看得到的啦
### 另外，这样的登录会持续一个月
### 详细的需要重新输入的时间见cookie的到期时间
### （所以说推荐重新登录哦）
###
-------------------------------------
```
[LuoGuCmd V0.1 (Alpha2) <By Micro>]
This is a free Luogu client for all OIer
The GPL protocol is used, and the source code is stored on Github.
> me
Hi,Micro
你的UID是：******

Micro - [******,***]
做过的题：
 已AC：
    P1*** - *****
 非AC：
    P1000 - 马利奥游戏
团队：
    T66666 :垃圾中的战斗机
> 

```
```
所以...~~登录功能还没做好~~提交代码功能还没做好->不能提交代码
但是以后一定可以的！一定！
然后用法在这下面：
-------------------------------------------------------
指令：
```
```
help（压根没写全，所有命令见本表，别看help）
```
```
login:
 - login
 详细过程请见输入后的提示
```
```
me:
  - me
  获取自身信息，需要登录，测试登录成功用这个，如果报错则不成功
```
```
setcookie:
  - setcookie <cookie>
  手动设置Cookie的值 (只能改一个，中间不能有空格,开发用)
```
```
getkey:
  - getkey [-shown]
  获得洛谷的x-csrf-token，以便登录时/提交代码时使用(目前废弃，开发用)
  加任意参数可以看见具体获得的东西
  ```
```
clear:
  - clear
  清屏，等同于Windows下cls
  ```
```
testdg:
  - testdg
  测试无参递归的最高次数
  报错前的次数即为可输入命令的最大次数
  （重启程序后最大次数会重置，最大次数大概2w次吧，所以没啥好担心的）
  （最大次数的报错是RangeError: Maximum call stack size exceeded，遇到该报错无需惊慌，重启程序即可）
```
```
user:
  - user <用户id>
  查看指定用户的详细信息
  有一个已知问题
```
```
loadcookie:
  - loadcookie <UMdid> <CNZZEid>
  已经废弃的命令
```
```
setkey:
  - setkey <x-token>
  手动设置token
  已经废弃的命令
```
```
fbnc:
  - fbnc <number>
  有参递归测试
  （递归求斐波那契）
  为什么叫fbnc而不是fbnq或fibonacci——因为我脑子抽了...
```
```
lookat:
  - lookat <题目编号>
  如:lookat P1000
  查看题目内容(图片不会显示)
  ```
```
chknew:
  - chknew
  检查更新
  还没做好，别用
  炸了我不管啊（逃
```

-------------------------------------------------------


如果有协同开发意愿，欢迎加QQ
~~（QQ自己源代码里面找去）~~
### 测试阶段，不会打包用到的包，请自行npm install
```
https
node-fetch
readline
cheerio
node-localstorage
```
-------------------------------------------------------

什么？你问我为神么要做这玩意？
~~只是为了好玩~~
当然是用！
洛谷有很多不方便的地方，比如团队赛题不实时更新，测试点有时要刷新之类的
所以做点改善

--------------------------------------------------------

### 代码随便用，但是如果你用了你也得开源！
~~（所以说为什么不一起做呢~~
#GPL协议
