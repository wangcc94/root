我的Github项目根目录


版本回退:git reset --hard commit_id

查看提交历史:git log

查看命令历史:git reflog

撤回暂存区到工作区:git reset HEAD fileName

撤销修改(回到最近一次git commit或git add时的状态):git checkout -- fileName

远程库->(连接)本地库:git remote add <origin> <url>

本地库->(推送)远程库:git push [-u] origin master

克隆:git clone <url>

查看分支：git branch

创建分支：git branch <name>

切换分支：git checkout <name>

创建+切换分支：git checkout -b <name>

合并某分支到当前分支：git merge <name>

删除分支：git branch -d <name>