# git

git 使用

.gitgnore 配置 git 忽略文件
#

配置git用户名 和邮箱
git config —global user.name “你的github使用”
git config —global user.email “你的额github邮箱”


git config —global -l  查看所有的配置
git config --global user.name


创建版本库
1.先建空目录
2.git init  初始化仓库
3.

touch 1.txt  
新建1.txt文件

//添加到暂存区
git add 1.txt
git add -A
//添加到历史区
git commit -m “备注信息”

//查看 历史记录
git log 


下载项目
git clone  地址

进去到 clone 的文件夹
cd 目录

推送到远程 ( 默认 有origin  和 master 分支)
git push origin master 
