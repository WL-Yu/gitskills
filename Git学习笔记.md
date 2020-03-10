## Git是什么

## Git的控制系统

## 建立版本库

## 创建远程仓库

https://github.com/WL-Yu/gitskills.git





## 创建仓库

### 步骤

创建一个空目录：

```
$ mkdir learngit   
$ cd learngit    
$ pwd			
/Users/michael/learngit
$ git init




```

![image-20200310170116042](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20200310170116042.png)



添加文件到Git仓库：

1. 使用命令`git add `，注意，可反复多次使用，添加多个文件；
2. 使用命令`git commit -m `，完成。



## 常用的Git命令

*  git config

设置Git行为和外观的工具

```bash
a) 查看用户配置
   $ git config --global –list

b) 配置用户名和邮箱
   $ git config --global user.name user-name
   $ git config --global user.email user-email
```

* git init

在当前目录新建Git代码仓库

```bash
$ git init
```

- git clone
  克隆Git仓库到本地

```bash
a) $ git clone URL

b) 克隆代码库到自定义目录
   $ git clone URL your-dir
```

- git status

查看文件状态

```bash
a) 标准输出
   $ git status

b) 简洁输出
   $ git status -s(或--short)
```

- git add
  跟踪新文件，或者把已跟踪的文件放入暂存区

```bash
a) 添加指定文件 
   $ git add filename

b) 添加匹配结果指定的文件
   $ git add *.c
```

- git diff

比较当前工作目录中文件和暂存区快照之间的差异。

```bash
a) 查看文件在工作目录和暂存区快照的差别
   $ git diff
b) 查看已经暂存起来的文件和上次提交时的快照之间的差异
   $ git diff --staged 
   $ git diff –cached
```

-  git rm
  移除文件

```bash
a) 从跟踪文件列表中清除，并从磁盘上删除文件
   $ git rm -f file-path
b) 从跟踪文件列表中清除，仍然将源文件保存在磁盘上
   $ git rm --cached file-path
```

-  git commit
  将更改从暂存区写入到Git仓库中

```bash
a) 正常提交
   $ git commit -m “desc”
   $ git commit -a -m “desc”

b) 追加提交
   $ git commit –amend -m “desc”
```

-  git remote
  查看远程仓库服务器

```bash
a) 显示远程服务器简写
   $ git remote
b) 显示读写远程仓库使用的Git保存的简写和对应的URL
   $ git remote -v
```

- git branch 
  分支操作命令

```bash
a) 查看分支
   $ git branch [-v]
b) 创建新分支
   $ git branch branch-name
c) 删除分支
   $ git branch -d branch-name
d) 查看哪些分支已经/仍未合并到当前分支
   $ git branch --merged
   $ git branch --no-merged
e) 建立追踪关系。
   $ git branch --set-upstream master origin/next
```

- git checkout

切换分支和创建分支

```bash
a) 当前分支切换到另一个分支
   $ git checkout other-branch
b) 创建新分支并切换到新分支
   $ git checkout -b new-branch
```









体会：对我来说，Git是一个完全陌生的东西，这两天的学习无疑是从0开始。在学习的过程中，有遇到许多问题，比如说网站404、看不懂指令等，但是在自己摸索和与伙伴讨论的过程中、收获了很多，自学能力和理解能力也提高了。同时，也坚定了要继续努力学习的决心。