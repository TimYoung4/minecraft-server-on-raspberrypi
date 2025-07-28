# 基于树莓派4B的我的世界游戏服务器搭建 Minecraft Server on Rastberry Pi 4B(4GB)
## 项目介绍 Project Description
使用树莓派 4B(4GB) + 外接 SSD 搭建轻量级 Minecraft Java Edition 服务器, 适用于1-5人同时在线, 以下以Windows为例作为协助<br>
Using Raspberry Pi 4B(4GB) + an external SSD to set up a lightweight Minecraft Java Edition server, suitable for small groups(1-5 players), following uses Windows as a example to help the setup
## 你需要什么 What will be needed
- 树莓派 4B(4GB)或更高端版本 Raspberry Pi 4B(4GB) or higher version
- 树莓派启动盘制作工具(用于Raspberry Pi OS(64-bit）的烧录）Raspberry Pi Imager(To set up the Operation System on the Raspberry Pi)<br>
  (下载地址 Downloadlink: https://www.raspberrypi.com/software/）
- SD卡(16GB） SD-card(16GB）
- 一台装有Xshell和VNC Viewer的电脑 a PC with Xshell and VNC viewer<br>
  (也可以使用其他ssh工具和可视化远程访问工具, other ssh tool and visialized remote control tool will also be fine)<br>
  (Xshell下载地址 Downloadlink for Xshell: https://xshell.com/en/xshell/)<br>
  (VNC Viewer下载地址 Downloadlink for VNC Viewer: https://www.realvnc.com/en/connect/download/viewer/?lai_vid=PXJnzM9V2HVzQ&lai_sr=0-4&lai_sl=l)<br>
## 搭建步骤 Setup Steps
### 1. 前期准备 Preparation
- 烧录树莓派系统 set up the Raspberry Pi OS
  - 插入SD卡并打开树莓派启动盘制作工具 insert the SD card to the PC and open the Raspberry Pi Imager
  - 选择正确的树莓派型号，此处选择的是RaspbarryPi4型号 choose the right Raspberry Pi Model, here uses RaspbarryPi4
  - 选择推荐的操作系统用于烧录 choose the recommanded OS(the first one) for the setup (Raspberry Pi OS x64)
  - 选择你插入的那张SD卡 choose the SD card for the device
  - 按下Ctrl+Shift+x来进行自定义设置 press Ctrl+Shift+x to open the further setup
    - 启用SSH服务并设置用户名和密码 enable the ssh service and set the Username and the Password
    - 可以设置一下网路 让树莓派能在开机后立刻连上路由器(网络) configure the WiFi, the one you're currently using, we want to let the Raspberry connects to the Router right after power on
    - 设置语言 然后保存 set the language and save
  - 点击烧录 then press 'Write'
- 获取树莓派IP地址 get the ip address of the Raspberry Pi
  - 按下Win+R输入cmd并执行 ipconfig命令 press Win+R and open 'cmd' and execute ipconfig
  - 找到默认网关 并记录下得到的IP地址 类似于(192.168.xxx.xxx) note down the ip address on the line 'Standardgateway', something like 192.168.xxx.xxx
  - 将最后一小节改成1 一般来说你就得到了你路由器的IP地址 change the last section of address to 1, like 192.168.xxx.1, should be the ip address of your Router
  - 将你得到的路由器IP地址粘贴到浏览器进入浏览器后台 密码一般在路由器里有写 and paste the router ip address to your browser, should open the backstage of your router, the password to the Router could be found in the back of the router
  - 将SD卡插到树莓派里 若绿灯不规律闪烁 那应该是成功了 insert the SD card to the Raspbarry Pi, if the green light blinks, shoulb be fine
  - 等待一小段时间 你能在路由器后台找到树莓派和对应的IP地址 这就是树莓派的IP地址 wait for a little bit, until you see the raspberrypi under the connected devices, and get the ip address of the Raspberry Pi
- 连接Xshell并为树莓派配置静态IP地址 connect with the Xshell and set the static ip for the Raspberry Pi
  - 打开Xshell并创建新的会话 在用户一栏输入得到的树莓派IP地址后连接 然后根据提醒输入之前设置的用户名密码进行访问 open the Xshell create a session with host of your Raspberry Pi ip address, then connect with username and the password you set earlier
 
# rest will coming up。。。<br>【【树莓派补完计划】4B启动！MC启动！用树莓派搭建属于自己的MC服务器】 https://www.bilibili.com/video/BV1Vx42197KH/?share_source=copy_web<br>This is a great Reference！！！
