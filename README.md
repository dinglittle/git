## git 使用

#### .gitgnore 配置 git 忽略文件
```
node_modules
.vscode
.babelrc
.idea/
package-lock.json


node_modules/
package-lock.json

```

#### 配置git用户名 和邮箱
```
git config —global user.name “你的github使用”
git config —global user.email “你的额github邮箱”

git config —global -l  查看所有的配置
git config --global user.name
```

#### 创建版本库
- 1.先建空目录
- 2.git init  初始化仓库
- 3.进入 目录操作

#### 添加远程项目地址
```
git remote add origin 地址
```

#### 新建1.txt文件
```
touch 1.txt  
```
#### 添加到暂存区
```
// 提交指定文件
git add 1.txt
// 提交全部文件
git add -A
```
#### 添加到历史区
```
git commit -m “备注信息”
```
#### 查看 历史记录
```
git log 
```

#### 下载项目
```
git clone  地址
```
进去到 clone 的文件夹
```
cd 目录
```
推送到远程 ( 默认 有origin  和 master 分支)
```
git push origin master 
```

==git 克隆下来 少文件==
直接 下载压缩包


#### git 创建远程分支

- 1)先在本地建分支
```
	git branch 分支名
```
- 2)切换到新的分支
```
	git checkout 分支名
```
- 3)将新的分支发布在github上
```
	git push origin 分支名
```
#### 在本地删除分支
```
gir branch -d 分支名 
//这里注意,要删除的分支不能是当前分支
```
#### 删除远程分支
```
git push origin :分支名
```
#### 合并分支  ( 将 develop 分支 合并到当前分支 ,注意 无法将 master主分支 合并到其他分支 )
```
git merge develop
```

---

#### git下回滚之前的 代码
业务需求:
	需要找到之前的指定提交代码
分析:
1)先找到要回滚的提交
2)拉一个新分支, 并指向 指定的 commit
```
git branch  [new branch] [commit]
```
3)切换到新分支,并拉取代码
```
git checkout new branch
```
4)提交新分支
```
git push origin new branch
```




