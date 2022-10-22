## Vscode安装
首先到vscode的官方下载网站 https://code.visualstudio.com/Download

<!-- tabs:start -->
### **Windows安装**
下载了Windows版本的vscode安装包后双击安装包且一直按Next就可以了
<div style="text-align:center;">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20220307184722/3.png"></img>
</div>
<div style="text-align:center;">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20220307184804/5.png"></img>
</div>
<div style="text-align:center;">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20220307184823/6.png"></img>
</div>

接下来就等它安装完就可以了

### **Linux安装**

- CentOS, RedHat

CentOS首先需要导入微软的GPG密钥，之后需要修改一个文件
```bash
sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc

sudo nano /etc/yum.repos.d/vscode.repo
```

将/etc/yum.repos.d/vscode.repo的内容改成以下那样就可以了
```bash
/etc/yum.repos.d/vscode.repo

[code]
name=Visual Studio Code
baseurl=https://packages.microsoft.com/yumrepos/vscode
enabled=1
gpgcheck=1
gpgkey=https://packages.microsoft.com/keys/microsoft.asc
```

最后执行以下命令就下载完成了
```bash
sudo yum install code
```

<br><br>

- Ubuntu, Debian

Ubuntu有两种方法安装，如果你之前安装过snap,那么就简单了，如果没有的话还有另一个方法下载Vscode

方法一 (下载过snap)
```bash
sudo snap install --classic code
```

方法二
```bash
sudo apt update

sudo apt install software-properties-common apt-transport-https wget -y

wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -

sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"

sudo apt install code
```

<br><br>

- Arch, Arco

```bash
sudo pacman -S visual-studio-code-bin
```

### **MacOS安装**
到了官网后选择Mac版本的安装包


下载完成后,双击安装包(有些会自动打开)，此时MacOS会显示提取文件中，当MacOS提取完后Vscode就会出现在同一个文件夹里

接下来打开另一个文件夹并找到应用程序(Application)并将Vscode拖拽进去，这样就能确保可以从Launch pad中打开Vscode

<!-- tabs:end -->