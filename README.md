# 这是我的设备！！最大化自定义 可开启功能：

# TSMS 
> 信息转发 TranspondSms， 把Android手动的短信通过邮件或者钉钉转出去

# 热点管理 
> 可设置跟随设备启动时启动热点，并且在热点关闭后10秒自动重启热点（所以想关闭热点先把设置页码的开启热点关掉）

博文连接[https://www.jianshu.com/p/608d1b1477e3]   APP下载 [https://pan.baidu.com/s/1kbelTFIf5nwkOY9g6itkvA]

--------
## 该工具实现特点和准则：
* **简单** 只做两件事：监听短信---》转发

由此带来的好处：
* 功能简单:（当时用Pad的时候，看手机验证码各种不方便，网上搜了好久也有解决方案）
> + AirDroid:手机管理工具功能太多，看着都耗电，权限太多，数据经过三方，账号分级
> + IFTTT:功能太多，看着耗电，权限太多，数据经过三方，收费
> + 还有些其他的也是这些毛病
* 省电：运行时只监听广播，有短信才执行转发，并记录最近n条的转发内容和转发状态
* 健壮：越简单越不会出错（UNIX设计哲学），就越少崩溃，运行越稳定持久

### 使用流程：
1. 在Android手机上安装TSMS 本APP后点击应用图标打开
2. + 点击钉钉转发后面的编辑按钮，在弹框中输入要转发的钉钉群自定义机器人的Token url，确认
   + 勾选钉钉转发选项即可启用钉钉群机器人转发短信
   + 使用邮箱转发同上配置邮箱smtp信息并勾选启用
3. 点击发送测试可用已勾选的配置发送消息到钉钉群或邮箱
4. 点击显示历史可查看已发送的历史记录


*注：该APP打开后会自动后台运行并在任务栏显示运行图标，请勿强杀，退出后请重新开启，并加入到系统白名单中*


### 应用截图：

![主界面](/pic/app.jpg "应用主界面")
![状态栏运行状态](/pic/taskbar.jpg "状态栏运行状态")
![钉钉机器人token设置](/pic/dingdingtokenset.jpg "钉钉机器人token设置")
![钉钉机器人转发](/pic/dingding.jpg "钉钉机器人转发")
![应用设置](/pic/setting.jpg "应用设置")

> v1.0 项目初始化，实现转发

> v1.1 减少手动配置启动参数：自启动配置、自动开启热点配置（设置好后手机重启也不用重新打开了，还能自动为pad开启热点）

