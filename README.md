# Git Command

**初始化仓库**

- `git init`                        当前目录创建为空的**Git本地存储库**
- `git add <file>`                  将文件提交到**stage暂存区**
  - `git add <file> <file>`         **多个文件**提交到stage暂存区
  - `git add .`                     提交目录下**所有文件**到stage暂存区
- `git rm --cached <file>`          stage暂存区内的文件**取消暂存**
- `git restore <file>`              放弃在**workspace工作区**中对stage暂存区文件的修改
- `git commit -m "create README.md"`提交**stage暂存区**中的文件到**Repository本地仓储**

**版本回溯**
`git log` 查看所有提交到本地仓库的记录 relog
`git log --graph`查看分支合并图
`git checkout -- file` 撤销工作区文件修改或误删
`git reset --hard <id>` 工作空间内容回溯到本地仓储指定提交记录

**分支管理**
`git branch` 查看本地仓库所有分支
`git branch <name>` 创建一个分支
`git checkout <name>`/`git switch <name>` 切换分支·
`git checkout -b <name>` / `git switch -c <name>` 创建并切换分支
`git merge <name>`合并指定分支到当前HEAD所在分支
`git branch -d <name>`删除分支
`git stash`保存当前分支内的stage暂存区内容
`git stash list`查看所有stage暂存区内容保存记录
`git stash apply stash@{num}`恢复stage暂存区内容到当前工作空间
`git stash drop`删除保存记录
`git cherry-pick <id>`将其他分支commit内容快速提交到当前分支 master分支出来的bug分支上的提交同样需要commmit到dev分支上

**多人协作分支管理**
`git switch -c dev origin/dev`创建本地dev分支和远程dev分支
`git push origin dev`推送dev分支到远程仓储
`git pull`拉取当前分支的远程仓储分支


**远程仓库管理**
`git remote -v`查看本地仓储关联的远程仓储
`git remote rm origin`删除本地仓储和远程仓储的关联 origin 远程仓储名称
`git remote add origin git@.....`关联远程仓储 
`git push -u origin master`推送master分支到远程仓储，并关联master分支，下次直接`git push` 


**git Config配置**

- `git config --local --list`               读取本地git配置信息
- `git config --glabal --list`              读取全局git配置信息
- `git config --local/--global user.name "<username>"` 设置配置项
- `git config --local/--global --unset user.name`      删除配置项


liuttttt
dddddddddddddddddddddddddddddddddddedededed
