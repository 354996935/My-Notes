### 生成密钥
    ssh-keygen -t rsa -C "354996935@qq.com"

#### 撤销已经push到远端的commit
    git log // 查看提交日志
    git reset --[参数] <版本号>
        --hard // 抛弃当前工作区的修改
        --soft // 回退版本后，保留修改，可重新提交
    git push origin <分支名> --force
        --force // (覆盖远端的版本信息)使远端的仓库也回退到相应的版本