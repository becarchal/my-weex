#
一个简单weex-app应用

[Weex](https://weex.apache.org/cn/)正如它的目标，可运行与ios，android，web三端

> 一套构建高性能、可扩展的原生应用的跨平台开发方案

Weex 给大家带来的无疑是客户端开发效率的提升，我们可以通过一套代码，实现web，android, iOS的三个平台上运行。

首先我们先来看下运行的效果吧:
以下是模拟器截图

**iOS 版**

<img src="https://github.com/becarchal/my-weex/blob/master/design_sketch/ios-sketch.png"/>

**Android 版**

<img src="https://github.com/becarchal/my-weex/blob/master/design_sketch/android-sketch.png"/>

**web 版**

<img src="https://github.com/becarchal/my-weex/blob/master/design_sketch/web-sketch.png"/>


*截图数据仅供参考*

###如何启动项目
``` bash
$ git clone
```
```
$ cd my-weex && npm install
```
or
```
cd my-weex && yarn
```
##### 参照官网[weex](https://weex.apache.org/cn/guide/integrate-to-your-app.html) 搭建开发环境
#####android：
安装[android studio](http://www.android-studio.org/) or androidSDK
配置sdk环境
可参照[react-native](https://reactnative.cn/docs/0.47/getting-started.html#content)官方sdk下载方法
```
vi .bash_profile
```
```
export ANDROID_HOME=/Users/[yourusername]/Library/Android/sdk
export PATH=$PATH:$ANDROID_HOME/tools:$ANDROID_HOME/platform-tools
```
方便以后开发可顺便在.bash_profile中添加如下快捷命令
```
alias wri="weex run ios"
alias wra="weex run android"
alias wrw="weex run web"

```
配置好后 终端输入
```
adb
```
看到如下信息：
```
Android Debug Bridge version 1.0.39
Version 0.0.1-4500957
Installed as /Users/binyang/Library/Android/sdk/platform-tools/adb

global options:
-a listen on all network interfaces, not just localhost
-d use USB device (error if multiple devices connected)
-e use TCP/IP device (error if multiple TCP/IP devices available)
-s SERIAL use device with given serial (overrides $ANDROID_SERIAL)
-t ID use device with given transport id
-H name of adb server host [default=localhost]
-P port of adb server [default=5037]
-L SOCKET listen on given socket for adb server [default=tcp:localhost:5037]

general commands:
devices [-l] list connected devices (-l for long output)
help show this help message
version show version num
......
```
则说明sdk安装成功。
提示：若在android studio运行时提示无法找到sdk，可参照[在Mac下为GUI程序设定环境变量](http://zodiacg.net/2013/05/set-path-under-mac/)重新设置sdk环境变量。

项目目录下运行
```
weex run android
```
or
```
wra
```
即可看到android效果如上图。
####ios:
在appstore安装xcode,参照[2017最新MacOS10.12安装CocoaPods参考步骤](https://www.jianshu.com/p/1b2d4040cd0c)安装CocoaPods

ios环境配置较为简单，即可在项目目录下运行
```
weex run ios
```
or
```
wri
```
即可看到ios效果如上图。

####web
在项目目录下运行
```
weex run web
```
or
```
wrw
```
即可看到web端效果如上图。


[my-weex](https://github.com/becarchal/my-weex),欢迎pullrequest,欢迎拍砖

### 扩展阅读

+ [weex-amap](https://github.com/weex-plugins/weex-amap)
+ [amap-running-app](https://github.com/weex-plugins/amap-running-app)
