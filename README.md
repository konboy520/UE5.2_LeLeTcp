# leletcp

* 昵称:马佳乐:wave::wave:
* 定位:用于本地连接tcp端口通讯并读取本地文件的插件 :round_pushpin: :round_pushpin:
* 简介：用于和公司枪械服务端进行通信并触发不同的事件，并把数据最后传递给服务端。
## 使用方法：
### 一.初次使用
1.放入项目Plugins目录中便可自动启动了
    2.点开项目内容浏览器插件目录的leletcp内容
    3.点开并把两个bp放入场景中便可食用
    ![](https://github.com/konboy520/UE5.2_LeLeTcp/new/main/img/image.png)
### 二.具体使用
1.点开BP_MyLeTcpClient蓝图后，可修改目标地址ip和端口
![](https://github.com/konboy520/UE5.2_LeLeTcp/new/main/img/image2.png)
    2.其他actor获取BP_MyLeTcpClient后绑定四个不同的事件和布尔值，可被服务端触发
    注意请在事件和方法中加入一点点延迟	:heavy_exclamation_mark:	:heavy_exclamation_mark:	:heavy_exclamation_mark:	:heavy_exclamation_mark:
![](https://github.com/konboy520/UE5.2_LeLeTcp/new/main/img/image3.png)
![](https://github.com/konboy520/UE5.2_LeLeTcp/new/main/img/image4.png)
    3.事件分为长按（按开，按中，按松），短按，最多有四个玩家在使用
![](https://github.com/konboy520/UE5.2_LeLeTcp/new/main/img/image5.png)
    4.点开BP_EndMyLeTcpClient，设置ip和端口
![](https://github.com/konboy520/UE5.2_LeLeTcp/new/main/img/image6.png)
    5.在你游戏逻辑结束时调用BP_EndMyLeTcpClient的事件EndEmit
![](https://github.com/konboy520/UE5.2_LeLeTcp/new/main/img/image8.png)
### 三.最后打包	:heavy_exclamation_mark:	:heavy_exclamation_mark:	:heavy_exclamation_mark:
把插件外的config.json放入打包后的项目名文件夹层级
![](https://github.com/konboy520/UE5.2_LeLeTcp/new/main/img/image7.png)
