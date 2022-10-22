## Pycharm安装
首先，到[pycharm官网](https://www.jetbrains.com/pycharm/download/)

<!-- tabs:start -->
### **Windows安装**
到了官网后选择社区版并下载，下载完后双击安装包并进入安装页面，后面一直按next就可以了

<br>
<div style="text-align:center;">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20200122121452/Pycharm-Windows-Installation-01.jpg"></img>
</div>

这里可以选择自己要下载在哪里
<div style="text-align:center;">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20200122121454/Pycharm-Windows-Installation-02.jpg"></img>
</div>

这里推荐除了第二行的选项外全部都勾选
<div style="text-align:center;">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20200122121457/Pycharm-Windows-Installation-03.jpg"></img>
</div>

这里直接选Next就可以了
<div style="text-align:center;">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20200122121500/Pycharm-Windows-Installation-04.jpg"></img>
</div>

接下来等它安装完就好了

### **Linux安装**

- Ubuntu, Debian, CentOS, Red Hat

首先到官网下载Linux版本的pycharm的社区版，然后打开终端输入

```bash
cd Downloads && tar xzf pycharm-*.tar.gz -C /opt/

cd /opt/pycharm-*/bin

chmod +x pycharm.sh

./pycharm.sh
```

?> 如果终端显示权限不足只需在前面加sudo就行了

<br><br>

- Arch, Arco

```bash
sudo pacman -S pycharm-community-edition
```

### **MacOS安装**
到了官网后选择社区版并下载

!> 这里注意，需要下载后缀为.dmg的那个

下载完成后,双击安装包(有些会自动打开),之后MacOS会显示一下图片

<div style="text-align:center;">
    <img src="../_media/mac_install_pycharm.png"></img>
</div>

这里只需要把pycharm的图标拖拽到右边显示的图标就可以了
<!-- tabs:end -->