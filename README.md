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

**分支管理**
`git branch` 查看本地仓库所有分支
`git branch -c/--copy` 复制一个分支和他所有relog

**git Config配置**

- `git config --local --list`               读取本地git配置信息
- `git config --glabal --list`              读取全局git配置信息
- `git config --local/--global user.name "<username>"` 设置配置项
- `git config --local/--global --unset user.name`      删除配置项
