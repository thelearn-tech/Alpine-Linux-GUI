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
(example **adduser pb** , **adduser thelearn-tech**)

**rc-service lightdm start**

as soon as you type **rc-service lightdm start** gui will start

and **login** promt will appear in login you will see ***Linux user*** and ***other..***

**login as** ***other..*** with the user name and password you set with ***adduser***
and enter ,now you will be in gui 

**As** you have login as user not root 
open terminal and type **su**
enter root password 
now you are **root**
and you can install use all stuff as root


when screensaver comes on press **space key** and in **linux user** give password **root**
or press **switch user** and login as **other** giving **username** and **password**

This was the first boot  
from now you can login as **Linux User** with password **root**
but it will be slow to load desktop enviroment
and in generall experience will be **slow**

**So** i will recommend you to login as **other**
expreance will be faster than if u login as **Linux User**

***NOTE***:- If you login as **Linux User** on screensaver
your **Experience will be same**


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

**ctrl + x**  (to save changes)

**y** (for yes)

**enter**(hit enter key)

**reboot**

After rebooting test if **fireefox** iss working by searching someting like **www.github.com**

# audio

For audio u can download **cmus** ,**gnome** , **MPV**


**apk add cmus**

**apk add gnome**  

**apk add mpv**


**No Sound Troubleshooting**

If you have no sound out that means there is no audio engine

**apk add pulseaudio**

**apk add alsa-utils alsa-utils-doc**

**apk add alsa-lib alsaconf**

**alsamixer**

**Esc** (press **Esc** key**

**rc-service alsa start**

**rc-update add alsa**

**reboot**


# Commands 

**note**:-you need to be **root** to install programs 


**poweroff**
(will turn of your PC)

**reboot** 
(will reboot your PC)


**rebooting** PC usualy solves alot of problems.

report problems and for more solution on
Alpine Linux [Discussion page](https://github.com/thelearn-tech/Alpine-Linux-GUI/discussion)

I may be late to reply but i  will reply

