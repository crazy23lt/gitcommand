# Git Command

**初始化仓库**

- `git init`                        当前目录创建为空的**Git本地存储库**
- `git add <file>`                  将文件提交到**stage暂存区**
  - `git add <file> <file>`         **多个文件**提交到stage暂存区
  - `git add .`                     提交目录下**所有文件**到stage暂存区
- `git rm --cached <file>`          stage暂存区内的文件**取消暂存**
- `git restore <file>`              放弃**wrokspace工作区**中的文件修改