
### init 安装系统更新
    
    sudo apt-get update

    sudo apt-get upgrade

### 修改文件权限
    chmod -R 777 /home/  可读、可写、可执行

### 文件目录
    /usr/local/

### 软件安装
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
    sudo apt-get install im-switch
    im-switch -s fcitx -z default
    sudo reboot

#### deb 使用gdebi
    安装　sudo apt-get install gdebi

#### 
    sudo apt-get install softname
    sudo apt-get update
    sudo apt-get -f install