## Pycharm Installation
First, go to [pycharm official website](https://www.jetbrains.com/pycharm/download/)

## Installation Guide

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

## Pycharm Configuration

After downloading pycharm we need to set up something to officially start.
When the download is complete, pycharm will automatically open, click on New Project
<div style="text-align:center;">
    <img src="../_media/pycharm_first.png"></img>
</div>

After that, you can set the folder name and folder location you want here
<div style="text-align:center;">
    <img src="../_media/pycharm_env.png"></img>
</div>

This is usually the case when you first open pycharm
<div style="text-align:center;">
    <img src="../_media/pycharm_first_enter.png"></img>
</div>

Here is a general description of some of the basic settings of pycharm.
First, find File > Settings in the upper left corner Windows users can use the shortcut Ctrl + Alt + s (Linux users who do not use window manager can also use this shortcut)

This page may be thought by ordinary people to be too small and unclear (anyway, I think it is too small), to set the font size, first find Editor, and then find Font
<div style="text-align:center;">
    <img src="../_media/pycharm_font.png"></img>
</div>

Here you can set the size of the font
<div style="text-align:center;">
    <img src="../_media/pycharm_font1.png"></img>
</div>

2. Some people may feel that the color of this pycharm is not very personal to their liking, then we can download the plugin to change the theme of pycharm
First, find Plugin and type theme in the search bar (if you have a personal favorite theme, you can also try to find it here)
There are a lot of different themes to choose from
<div style="text-align:center;">
    <img src="../_media/pycharm_theme.png"></img>
</div>

I personally prefer the theme of Palenight, so here I will download Palenight, choose the theme you want, click it, and find install and click
<div style="text-align:center;">
    <img src="../_media/pycharm_theme_install.png"></img>
</div>

!> A pop-up window may pop up here, just click Accept
<div style="text-align:center;">
    <img src="../_media/pycharm_install_theme.png"></img>
</div>

So at this point, it's basically done, and then we can start writing code