# 这是一个没做完的洛谷CMD客户端 #

~~它实现了**非原生的登录**
可 是
有点麻烦
因为洛谷使用了__client_id的验证，这需要我一直连接以保证这个id不失效（断开连接即ID失效）
但是我这个垃圾不会不断开连接...我怎么办！我能怎么办！（要是有dalao会的话，请联系我！~~
登录功能我选择放弃QwQ（下午又炸了一次
所以说我选择曲线救国~~（分明就是懒嘛~~
目前的方式是在洛谷主页登录后拿到Cookie，输入cookie以登录
A2 等我好消息！
目前登录可以做到这一步了：~~（洛谷第三方客户端的长足进步~~
*是手动隐藏，到时候看得到的啦

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
 - login <帐号> <密码>
 或
 - login（记忆帐号登录，没做完）
 因为我搞不定__client_id所以说这玩意你得手动获取，获取方式是在洛谷页面打开Chrome开发者模式，network里面随便选一个请求，找到__client_id=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx，将xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx替换掉 var Cookie=后面那个[clientid]，[youruid]填你的洛谷id
```
```
me:
  - me
  获取自身信息，需要登录，测试登录成功用这个，如果报错则不成功或者[youruid]没写
```
```
setcookie:
  - setcookie <cookie>
  改Cookie的值，只能改一个，中间不能有空格
```
```
getkey:
  - getkey [-shown]
  获得洛谷的x-csrf-token，以便登录时/提交代码时使用
  加任意参数可以看见具体获得的东西
  ```
```
clear:
  - clear
  清屏，等同于Windows下cls
  ```
```
lookat:
  - lookat <题目编号>
  如:lookat P1000
  查看题目内容(图片不会显示)
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
