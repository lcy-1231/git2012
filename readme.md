
# GIT 使用

工作区 - 暂存区 - 本地仓库

1. 在电脑上创建一个文件夹作为工作区
2. 打开文件夹右键 git base here 进入当前目录
3. 工作区持有项目实际文件

## readme 文档
1. readme 文件可以是txt文档，也可以是md文档
2. 作用:一般和项目放在一起，作为项目的说明文档

## 全局配置
1. 配置用户名 git config --global user.name "你的git名称"
2. 配置邮箱   git config --global user.email "你的git验证邮箱"
3. 一台电脑配置一次就可以了
4. 查看你的配置信息 git config --list

## 初始化
1. 命令 git init 初始化版本仓库
2. 当前目录路径后面有(master)代表初始化成功
3. 在当前目录下生成一个隐藏文件 .git 代表这是一个版本库 
4. 不要操作，不要修改 .git 文件，让它隐藏

## 工作区内容提交到本地仓库
1. 执行命令 git add 文件名 将工作区的内容提交到暂存区
2. 命令 git add . 将所有变动(新增、修改、删除)提交到暂存区
3. 从暂存区提交到本地仓库 git commit -m '提交注释'

## 版本回退
1. 命令 git reset --hard HEAD^ 回退到上一个版本(一个^代表上一个版本)
2. 命令 git reset --hard 版本号 回退到指定版本


## 辅助命令
1. 命令 git status 查看当前目录下的操作状态(新增、修改、删除)
2. git log 查看日志 (提交记录，查看信息) 哈希值，指针，指向当前版本 查看版本号
3. git reflog 查看简版日志 7位简版本号



第XX版本

## 将本地仓库提交到远程仓库
1. 在github创建一个远程仓库 git2010
2. 本地工作区先提交到本地仓库
3. 命令 git remote add origin 远程仓库地址 ->本地仓库和远程仓库关联  (origin变量，指向远程地址)
4. 命令 git remote -v 查看本地仓库
5. 命令 git push -u origin master(主干，主分支) 
  git push 把本地仓库推送到远程仓库
  -u origin master  ->设置默认提交master分支到origin

## 下载项目到本地
1. 克隆项目: git clone 地址
2. cd GP03-test/ 有master 直接是一个版本库了
3. git clone 适用于本地没有该项目，直接从远程下载到本地
4. 如果本地有该项目，应该直接更新到本地 git pull
5. 一定要先把工作区的修改提交到本地在仓库再更新远程到本地

我在远程仓库修改的这句话 

## 分支操作
1. 查看当前仓库的所有分支 git branch
2. 当前分支前面带有 星号 *
3. 创建分支 git branch 分支名
4. 切换分支 git checkout 分支名
5. 切换分支之后，工作区显示的是 当前分支的代码
6. 合并分支 git merge test
7. 删除分支 git branch -d test

test分支的代码 要提交

此时还没有修改这里，我修改了这里


没修改不让提交
我是test新增的功能！！！我的master还能回来吗？？
