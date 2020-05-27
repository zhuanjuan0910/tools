# git版本控制工具的使用
## Git的安装（以乌班图系统为例）
```markdown
sudo apt install git
```
## git工作流程
+ git clone 资源库作为工作目录
+ 在工作目录上对文件进行增删改查
+ git status 查看文件状态
+ git push 推送文件到远程仓库
## 工作区，暂存区，版本库
+ 工作区是当前工作目录
+ git add 之后加入暂存区
+ git commit 提交入版本库
## 创建仓库
+ git init 初始化一个仓库，生成.git文件
+ git clone 克隆仓库
## git的基本操作
+ git add . 把当前目录下的所有文件加入缓存区
+ git commit 将缓存区的内容添加到仓库中
+ git commit -a 可跳过git add这步
+ git commit -m 提供提交注释
+ git diff 已写入缓存与已修改尚未写入缓存的区别
+ git status 查看文件的修改状态
+ git mv 移动文件或对文件重命名
+ git rm 删除工作目录中的文件
+ git rm --cached file 从暂存区移除文件，工作区仍然保留
+ git reset HEAD file 取消已缓存的内容
+ git reset --hard 版本号，回滚到指定版本
## 分支管理
+ git branch brachname 创建分支
+ git checkout branchname 切换分支
+ git branch -d branchname 删除分支
+ git merge 合并分支
+ 合并冲突需要手动解决，并用git add告知冲突已解决
+ git branch 列出分支
+ git checkout -b branchname 创建分支并立即切换到该分支
## 查看提交历史
+ git log
+ git log --oneline 简洁的版本
+ git log --reverse 逆向显示所有日志
## 标签
+ git tag -a 
## git远程仓库
+ 添加远程仓库
```
git remote add [shortname] [url]
```
+ git remote 查看远程仓库
+ git fetch 从远程仓库下载新分支与数据
+ git merge 从远端仓库提取数据并尝试合并到当前分支
+ git push [alias] [branch]推送数据到远程仓库
+ git remote rm [别名]删除远程仓库
+ git pull <远程主机名><远程分支名>取回远程主机的某个分支，再与本地的指定分支合并


