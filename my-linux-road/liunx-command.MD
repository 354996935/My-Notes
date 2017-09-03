### .tar.xz 文件解压
    sudo xz -d ***.tar.xz
    sudo tar -xvf  ***.tar
    解压后在　/bin 文件夹下　已经安装好　但是是局部的
    设置全局　(local/bin 下面是全局)
    ln -s /home/zhengyf/mysofltware/node-v0.10.28-linux-x64/bin/node /usr/local/bin/node
    ln -s /home/zhengyf/mysofltware/node-v0.10.28-linux-x64/bin/npm /usr/local/bin/npm