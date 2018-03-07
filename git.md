Git 操作说明


配置用户名

git config --global user.name "your GitHub Account"

配置邮箱

git config --global user.email "your GitHub registed email"

版本库

创建版本库

在合适的地方，创建一个空目录，cd进入该目录，使用

git init 命令把这个目录变成Git可以管理的仓库

在仓库中vim创建一个git.md文件	添加 This is my first operate Git 为内容

把文件添加到仓库 命令

git add git.md

把文件提交到仓库 命令

git commit -m "注释信息"

查看当前仓库状态 命令

git status

查看修改内容 命令

git diff

----------------------------------------------------------------------------

远程仓库

创建SSH Key

输入 ssh-keygen -t rsa -C "your GitHub registed email"

记录.ssh目录位置

.ssh
|--id_rsa	私钥
|--id_rsa.pub	公钥

将公钥绑定在自己注册的GitHub上

测试秘钥是否通过

ssh -T git@github.com

github上的钥匙变绿说明链接成功


关联远程仓库 命令

git remote add origin 远程仓库地址

eg:

git remote add origin git@github.com:Miracle2Future/gitStation.git

推送本地仓库内容到远程仓库 命令

git push origin master

拉去远程库内容到本地库：

git pull origin master

从远程库克隆：

git clone 远程库地址

eg:	git clone git@github.com:Miracle2Future/gitStation.git





