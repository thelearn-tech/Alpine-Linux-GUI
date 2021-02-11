# Alpine-Linux-GUI
How to install GUI on Alpine Linux

# Installation

**apk add xf86-video-vesa**

**apk add xf86-input-mouse**

**apk add xf86-input-keyboard**

**apk update**

**apk add xfce4**

**apk add xfce4-terminal**

**apk add lightdm-gtk-greeter**

**apk add xfce-polkit**

**apk add xfce4-screensaver**

**apk add consolekit2**

**apk add sudo**

**rc-update add dbus**

**rc-service dbus start**

**rc-update add lightdm**

**adduser >username<**

**rc-service lightdm start**

as soon as you type **rc-service lightdm start** gui will start

and **login** promt will appear in login you will see ***Linux user*** and ***other..***

**login as** ***other..*** with the user name and password you set with ***adduser username***
and enter ,now you will be in gui 

**As** you have login as user not root 
open terminal and type **su**
enter root password 
now you are **root**
and you can install use all stuff as root

# Browser

i will recommend **Firefox** as its light weight

**apk add firefox-esr**

Now if u get ***server not found*** error in **Firefox**

You need to configure your DNS


open **terminal**

**su** (enter root password)

**apk add nano**

**cd /etc**

**nano resolv.conf**

![](https://raw.githubusercontent.com/thelearn-tech/Alpine-Linux-GUI/main/IMG_20210211_144126.jpg)


change nameserver 192.168.42.123
 to
namesever 8.8.8.8
![](https://raw.githubusercontent.com/thelearn-tech/Alpine-Linux-GUI/main/IMG_20210211_143918.jpg)

![](https://raw.githubusercontent.com/thelearn-tech/Alpine-Linux-GUI/main/IMG_20210211_143854.jpg)

**ctrl + x**

**y**

**enter**

**reboot**
After rebooting test if **fireefox** iss working by searching someting like **www.github.com**
