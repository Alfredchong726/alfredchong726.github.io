## Vscode Installation
Start by going to the vscode's official download site https://code.visualstudio.com/Download

## Installation Guide

<!-- tabs:start -->
### **Install in Windows**
After downloading the Windows version of the vscode installation package, double-click the installation package and press Next all the time
<div style="text-align:center;">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20220307184722/3.png"></img>
</div>
<div style="text-align:center;">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20220307184804/5.png"></img>
</div>
<div style="text-align:center;">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20220307184823/6.png"></img>
</div>

Then just wait for it to be installed

### **Install in Linux**

- CentOS, RedHat

CentOS first needs to import Microsoft's GPG key, then it will needs to modify a file
```bash
sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc

sudo nano /etc/yum.repos.d/vscode.repo
```

Change the contents of /etc/yum.repos.d/vscode.repo to the following
```bash
/etc/yum.repos.d/vscode.repo

[code]
name=Visual Studio Code
baseurl=https://packages.microsoft.com/yumrepos/vscode
enabled=1
gpgcheck=1
gpgkey=https://packages.microsoft.com/keys/microsoft.asc
```

Finally, execute the following command to download the download:
```bash
sudo yum install code
```

<br><br>

- Ubuntu, Debian

Ubuntu has two ways to install, if you've installed snap before, it's easy. If not, there's another way to download Vscode

Method 1 (downloaded snap)
```bash
sudo snap install --classic code
```

Method 2
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

### **Install in MacOS**
After arriving at the official website, select the installation package for the Mac version


After downloading, double-click on the installation package (some will open automatically), MacOS will display the extracted files, and Vscode will appear in the same folder when MacOS has finished extracting.

Next open another folder and find Applications and drag and drop Vscode into it to ensure that Vscode can be opened from the Launch pad.

<!-- tabs:end -->

## Vscode Configuration

After downloading Vscode, it cannot be used to write code for the time being, and several plugins need to be installed.
First, find this icon in the left action bar and click on it

<div style="text-align:center;">
    <img src="../_media/extension.png"></img>
</div>

After that enter python in the search bar and find the following plugin to download
<div style="text-align:center;">
    <img src="../_media/python_extension.png"></img>
</div>

Next, go back to the search bar and type code runner to search and download the following plugin
<div style="text-align:center;">
    <img src="../_media/code_run_extension.png"></img>
</div>

Once that's done, we can get started