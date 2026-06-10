# 安装Python

*最后编辑于2026/06/07 by:nood*

## Windows
*此处演示电脑配置:win1064位 最后编辑于2026/06/07 by:nood*

ok首先我们要先了解一下架构是什么意思 我们就说win常见的32位(x86)和64(x86-64)位 在目前 win11也就是目前win最新版本的架构为64位 如果你的电脑为win11系统 那你需要下载64位的软件 其他系统可以打开设置/控制面板查看架构

### 下载py

截至本文发布时 最新版本是3.14.5 64位点击[此处](https://www.python.org/ftp/python/3.14.5/python-3.14.5-amd64.exe)下载 32位点击[此处](https://www.python.org/ftp/python/3.14.5/python-3.14.5.exe)下载

### 安装

这里会带你一步一步安装 注意安装界面全英文 请仔细看下面
- 将下载好的.exe文件双击运行
- 在双击完成以后 在第一个界面选择Customize installation 也就是自定义安装 也可以看图标亮区域
![py环境安装1](/images/config/win/env/pyinstall1.PNG)
- 在这个页面 像下方图片一样全勾上就行了 然后点击图片中标亮按钮Next进入下一个页面
![py环境安装2](/images/config/win/env/pyinstall2.PNG)
- 在这个页面 像下方图片一样图片勾哪里你就也勾上 在Customize install location 是安装路径选择的地方 你可以在那个输入框中直接写路径 不过面缶还是建议你单击下方图片中标亮按钮 Browse 用图形化路径选择界面进行选择 选择好路径 单击下方图片中标亮的 Install 按钮 进行安装
![py环境安装3](/images/config/win/env/pyinstall3.PNG)
- 点击 Install 按钮后会出现一个用户账户控制界面 在那个窗口中选择图片中按钮 是 继续进行安装
![py环境安装4](/images/config/win/env/pyinstall4.jpg)
- 等进度条跑完 就安装成功了
![py环境安装5](/images/config/win/env/pyinstall5.PNG)
- 出现跟下方图片一样的界面 就说明安装成功了 单击 Close 按钮即可结束安装
![py环境安装6](/images/config/win/env/pyinstall6.PNG)

## Android Termux

*本文演示设备配置:Android16 最后编辑于2026/06/07 by:nood*

我们需要用到1个软件 Termux

然后我们打开Termux 输入:
```bash
pkg update && pkg upgrade -y
pkg install python -y
```

## 开始

现在找一个文件夹(Windows的不要放在C盘并且在资源管理器打开文件扩展名 Android的放在/storage/emulated/0/目录 Android你可以使用MT管理器 最好是新建一个文件夹 不要放在软件那些路径) 新建一个文件并命名为main.py 正式开始写吧