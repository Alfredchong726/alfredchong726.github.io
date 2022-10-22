## Pycharm Installation
First, go to [pycharm official website](https://www.jetbrains.com/pycharm/download/)

<!-- tabs:start -->
### **Install in Windows**
After arriving at the official website, select the community version and download, double-click the installation package and enter the installation page, and then press next

<br>
<div style="text-align:center;">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20200122121452/Pycharm-Windows-Installation-01.jpg"></img>
</div>

Here you can choose where you want to download it
<div style="text-align:center;">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20200122121454/Pycharm-Windows-Installation-02.jpg"></img>
</div>

It is recommended to check all except the options in the second row
<div style="text-align:center;">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20200122121457/Pycharm-Windows-Installation-03.jpg"></img>
</div>

Just choose Next here
<div style="text-align:center;">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20200122121500/Pycharm-Windows-Installation-04.jpg"></img>
</div>

Then, just wait for it to be installed

### **Install in Linux**
- Ubuntu, Debian, CentOS, Red Hat

First go to the official website to download the community version of pycharm for Linux, and then open the terminal to enter

```bash
cd Downloads && tar xzf pycharm-*.tar.gz -C /opt/

cd /opt/pycharm-*/bin

chmod +x pycharm.sh

./pycharm.sh
```

?> If the terminal shows insufficient permissions, just add sudo in front

<br><br>

- Arch, Arco

```bash
sudo pacman -S pycharm-community-edition
```

### **Install in MacOS**
After arriving at the official website, select the Community Edition and download it

!> Note here that you need to download the one with the suffix .dmg

After downloading, double-click the installation package (some will open automatically), after which MacOS will display a picture.

<div style="text-align:center;">
    <img src="../_media/mac_install_pycharm.png"></img>
</div>

Here you only need to drag and drop the pycharm icon to the icon displayed on the right
<!-- tabs:end -->
