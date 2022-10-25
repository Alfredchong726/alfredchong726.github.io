工欲善其事，必先利其器！！！

在学习编写代码之前，首先必须安装好所有必须的软件并将开发环境配置好，只有将这些事事情完成之后我们才能更高效地用代码实现相应的功能。这里会对环境配置进行详细说明。

- [Python安装](#python安装)
- [Pycharm安装](#pycharm安装)
- [Vscode安装](#vscode安装)

## Python安装
既然要使用Python,那么就需要到官网下载Python3。

[Python官网](https://www.python.org/) <br>
[Python下载地址](https://www.python.org/downloads/) <br>
[Python官方文档(中文版)](https://docs.python.org/zh-cn/3/) <br>
[Python第三方库](https://pypi.org/)

<!-- tabs:start -->

### **Windows安装**
1. 首先通过以上的下载地址到下载页面并点击一下按钮
<div style="text-align:center;">
    <img src="../_media/python_page.png"></img>
</div>
下载完后双击安装包开始下载python

2. 这里需要注意一个点

!> **一定一定**要点击add to path的选项

<div style="text-align:center;">
    <img src="../_media/python_add_path.png"></img>
</div>

1. 接下来验证是否下载成功
首先点击win按键(就是键盘上有一个window图案的按键)，输入cmd，回车，之后输入python并回车测试一下能否调用python,测试成功结果如下
<div style="text-align:center;">
    <img src="../_media/cmd.png"></img>
</div>


### **Linux安装**
- CentOS, RedHat

```bash
sudo yum install -y https://centos7.iuscommunity.org/ius-release.rpm

sudo yum update

sudo yum install -y python35u python35u-libs python35u-devel python35u-pip
```

<br><br>

- Ubuntu,Debian

```bash
sudo apt-get install -y python3-dev build-essential libssl-dev libffi-dev libxml2 libxml2-dev libxslt1-dev zlib1g-dev libcurl4-openssl-dev

sudo apt-get install python3 

sudo apt-get install python3-pip
```

<br><br>

- Arch, Arco

```bash
sudo pacman -S python3 python3-pip
```

#### 测试是否安装成功
在命令行中测试是否安装成功
<div style="text-align:center;">
    <img src="../_media/python_linux_test.png"></img>
</div>


### **MacOS安装**
使用MacOS的应该都知道brew,brew是Mac平台下强大的软件管理工具，官方网站为 https://brew.sh/index_zh-cn

1. 首先执行以下命令行下载brew
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

2. 接着就使用brew来安装python
```bash
brew install python3
```

3. 测试是否安装成功
```bash
~python3
python 3.6.1 (default, Apr 4 2017, 09:40:21)
[Gcc 4.2.1 Compatible Apple LLVM 8.1.0(clang-802.0.38)] on darwin
Type "help" , "copyright" "credits" or "license" for more information.
```
<!-- tabs:end -->

那么现在python下载完了，接下来就需要一个合适的IDLE,当然也可以使用python自带的IDLE
<br>
<div style="text-align:center;">
    <img src="https://i.ytimg.com/vi/nRYi05ECI04/maxresdefault.jpg"></img>
</div>

可是这里并不建议使用python自带的IDLE，因为还有更好的选择。
这里推荐下载pycharm或者vscode

这里先说说个人比较推荐哪一个，个人还是比较推荐vscode的。Pycharm的确很强大，我曾经试用pycharm专业版，的确是很好用，身边也是很多人推荐用这款IDLE。可是本人秉持着能白嫖绝不花钱的理念还是放弃了pycharm专业版并转行到pycharm社区版。可是pycharm社区版有很多限制，有许多功能都没办法使用。
<br><br>
后来我就换成了NeoVim，可是这个对新手来说非常地不友好，所以在这里就没有推荐。提一嘴，NeoVim也是非常好用哦，就是出bug的时候绝对要你一大撮头发就对了。
<br><br>
vscode即免费，里面提供的插件也非常多(绝对多过pycharm)，所以这里我站vscode。
<br><br>
当然，p如果你是大佬，不介意花钱买pycharm专业版就当我没说

这里有提供Pycharm和Vscode的安装以及设置
- [Pycharm安装](../pycharm.md)
- [Vscode安装](../vscode.md)