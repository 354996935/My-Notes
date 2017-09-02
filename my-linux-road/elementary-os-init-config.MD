
---
    title: How to configure and use elementary OS
    author: zhengyf
    createdTime: 2017/09/02
---

### init 安装系统更新
    sudo apt-get update
    sudo apt-get upgrade

### 软件安装
    sudo apt-get install softname
    sudo apt-get update
    sudo apt-get -f install

#### chrome
    wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
    sudo dpkg -i google-chrome*; 
    sudo apt-get -f install // 解决依赖关系

#### 输入法
    sudo apt-get removeibus
    sudo add-apt-repository ppa:fcitx-team/nightly
    sudo add-apt-repository ppa:fcitx-team/stable
    sudo apt-get update
    sudo apt-get install fcitxfcitx-config-gtk fcitx-googlepinyin
    sudo apt-get install fcitx-table-all
    sudo apt-get install im-switch　// (im-config 非必须)
    im-switch -s fcitx -z default
    sudo reboot

#### .deb文件 使用gdebi
    安装　sudo apt-get install gdebi
    右键deb包　选择gdebi打开

### 软件文件目录（一般）
    /usr/local/

### 修改文件权限
    chmod -R 777 /home/  可读、可写、可执行
