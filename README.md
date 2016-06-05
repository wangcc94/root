我的Github项目根目录

创建ssh_key:ssh-keygen -t rsa -C "youremail@example.com"

创建库:git init

版本回退:git reset --hard commit_id

查看提交历史:git log

查看命令历史:git reflog

撤回暂存区到工作区:git reset HEAD fileName

撤销修改(回到最近一次git commit或git add时的状态):git checkout -- fileName

远程库->(连接)本地库:git remote add <origin> <url>

更改远程库地址:git remote <origin> set-url <url>

删除远程库地址:git remote rm <origin>

分支建立链接://git branch --set-upstream <dev> <origin>/<dev>
//git branch --set-upstream-to origin/dev dev

本地库->(推送)远程库:git pull

本地库->(拉取)远程库:git push [-u] origin master

本地获取远程库分支:git checkout -b branch-name origin/branch-name

克隆:git clone <url>

查看分支：git branch

创建分支：git branch <name>

切换分支：git checkout <name>

创建+切换分支：git checkout -b <name>

合并某分支到当前分支：git merge <name>

删除分支：git branch -d <name>

非快速合并(Fast forward)到当前分支:git merge --no-ff -m "描述" <name>

工作区贮藏:git stash

贮藏列表:git stash list

工作区恢复:git stash apply stash@{0};
            git stash pop
            
查看远程分支:git ls-remote --heads origin

创建标签:git tag <name>
//git tag -a/-s <name> -m "info"

查看标签:git tag
git show <name>

删除标签:git -d <name>

推送标签:git push origin <name>
//git push origin --tags

删除远程标签:git push origin :refs/tags/<name>

忽略文件:.gitignore

强制添加文件:git add -f fileName

检查忽略文件:git check-ignore -v fileName

配置别名:git config --global alias.lg "log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit"