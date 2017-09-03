### .tar.xz 文件解压
    sudo xz -d ***.tar.xz
    sudo tar -xvf  ***.tar
    解压后在　/bin 文件夹下　已经安装好　但是是局部的
    设置全局　(local/bin 下面是全局)
    ln -s /home/zhengyf/mysofltware/node-v0.10.28-linux-x64/bin/node /usr/local/bin/node
    ln -s /home/zhengyf/mysofltware/node-v0.10.28-linux-x64/bin/npm /usr/local/bin/npm

### .tar.gz 文件解压安装
    sudo tar -zxvf smartgit-linux-17_0_5.tar.gz (解压)
    ./bin/smartgit.sh

### 配置java环境变量
    下载jdk .tar.gz 包
    解压jdk到当前目录,得到文件夹 jdk1.8.0_*
    tar -zxvf jdk-8u60-linux-x64.tar.gz
    
    安装完毕为他建立一个链接以节省目录长度
    ln -s /usr/local/soft/jdk1.8.0_144 /usr/jdk

    编辑配置文件，配置环境变量
    vim /etc/profile
    在文本的末尾添加如下内容：

    JAVA_HOME=/usr/jdk
    CLASSPATH=$JAVA_HOME/lib/
    PATH=$PATH:$JAVA_HOME/bin
    export PATH JAVA_HOME CLASSPATH

    重新启动
    java -version　(查看版本)