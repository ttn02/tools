Git使用教程

初始化为仓库：git init

查看仓库状态：git status

添加文件到暂存区：git add （文件或“.”添加全部文件）

提交文件到仓库：git commit -m （文件）

### 1. 安装 Git

首先，你需要在你的计算机上安装 Git。

- **Windows**: 下载并安装 [Git for Windows](https://git-scm.com/download/win)。
- **macOS**: 使用 Homebrew 安装：`brew install git`。
- **Linux**: 使用包管理器安装，例如在 Ubuntu 上：`sudo apt-get install git`。

### 2. 配置 Git

安装完成后，你需要配置你的用户名和电子邮件地址，这些信息会记录在你的提交中。

```
git config --global user.name "ttn"
git config --global user.email "3442322864@qq.com"
```

### 3. 创建仓库

你可以创建一个新的 Git 仓库，或者克隆一个已有的仓库。

- **初始化新仓库**:

  ```
  git init
  ```

  这会在当前目录创建一个新的 Git 仓库。

- **克隆已有仓库**:

  ```
  git clone <仓库URL>
  ```

  这会将远程仓库克隆到本地。

### 4. 基本操作

- **查看状态**:

  ```
  git status
  ```

  查看工作目录和暂存区的状态。

- **添加文件到暂存区**:

  ```
  git add <文件名>
  ```

  或者添加所有更改的文件：

  ```
  git add .
  ```

- **提交更改**:

  ```
  git commit -m "提交信息"
  ```

  提交暂存区的更改到本地仓库。

- **查看提交历史**:

  ```
  git log
  ```

  查看项目的提交历史。

### 5. 分支管理

- **创建新分支**:

  ```
  git branch <分支名>
  ```

- **切换分支**:

  ```
  git checkout <分支名>
  ```

- **创建并切换分支**:

  ```
  git checkout -b <分支名>
  ```

- **合并分支**:

  ```
  git merge <分支名>
  ```

  将指定分支合并到当前分支。

- **删除分支**:

  ```
  git branch -d <分支名>
  ```

### 6. 远程仓库

- **添加远程仓库**:

  ```
  git remote add origin <仓库URL>
  ```

- **推送到远程仓库**:

  ```
  git push origin <分支名>
  ```

- **从远程仓库拉取更新**:

  ```
  git pull origin <分支名>
  ```

### 7. 其他常用命令

- **撤销工作区的更改**:

  ```
  git checkout -- <文件名>
  ```

- **撤销暂存区的更改**:

  ```
  git reset HEAD <文件名>
  ```

- **查看差异**:

  ```
  git diff
  ```

  查看工作区和暂存区的差异。

  ```
  git diff --cached
  ```

  查看暂存区和最后一次提交的差异。

### 8. 标签

- **创建标签**:

  ```
  git tag <标签名>
  ```

- **查看标签**:

  ```
  git tag
  ```

- **推送标签到远程仓库**:

  ```
  git push origin <标签名>
  ```

  或者推送所有标签：

  ```
  git push origin --tags
  ```

### 9. 忽略文件

你可以创建一个 `.gitignore` 文件来指定哪些文件或目录应该被 Git 忽略。

```
# 忽略所有 .log 文件
*.log

# 忽略 node_modules 目录
node_modules/
```

### 10. 撤销提交

- **撤销上一次提交**:

  ```
  git reset --soft HEAD^
  ```

  撤销提交但保留更改。

  ```
  git reset --hard HEAD^
  ```

  撤销提交并丢弃更改。

### 11. 储藏更改

如果你在当前分支上有未提交的更改，但需要切换到其他分支，可以使用 `git stash` 来储藏这些更改。

- **储藏更改**:

  ```
  git stash
  ```

- **恢复储藏的更改**:

  ```
  git stash apply
  ```

### 12. 查看远程仓库信息

- **查看远程仓库**:

  ```
  git remote -v
  ```

- **查看远程仓库详细信息**:

  ```
  git remote show origin
  ```

### 13. 重命名分支

- **本地分支重命名**:

  ```
  git branch -m <旧分支名> <新分支名>
  ```

- **删除远程分支并推送新分支**:

  ```
  git push origin --delete <旧分支名>
  git push origin <新分支名>
  ```

### 14. 查看文件历史

- **查看文件的提交历史**:

  ```
  git log <文件名>
  ```

- **查看文件的更改历史**:

  ```
  git blame <文件名>
  ```

### 15. 子模块

Git 子模块允许你将一个 Git 仓库作为另一个 Git 仓库的子目录。

- **添加子模块**:

  ```
  git submodule add <仓库URL> <路径>
  ```

- **初始化子模块**:

  ```
  git submodule init
  ```

- **更新子模块**:

  ```
  git submodule update
  ```

### 16. 清理仓库

- **清理未跟踪的文件**:

  ```
  git clean -f
  ```

- **清理未跟踪的目录**:

  ```
  git clean -fd
  ```

### 17. 查看配置

- **查看所有配置**:

  ```
  git config --list
  ```

- **查看特定配置**:

  ```
  git config <配置项>
  ```

### 18. 修改最后一次提交

- **修改最后一次提交信息**:

  ```
  git commit --amend
  ```

- **修改最后一次提交内容**:

  ```
  git add <文件名>
  git commit --amend
  ```

### 19. 查看远程分支

- **查看所有远程分支**:

  ```
  git branch -r
  ```

- **查看所有本地和远程分支**:

  ```
  git branch -a
  ```

### 20. 删除远程分支

- **删除远程分支**:

  ```
  git push origin --delete <分支名>
  ```

### 21. 查看差异

- **查看工作区和暂存区的差异**:

  ```
  git diff
  ```

- **查看暂存区和最后一次提交的差异**:

  ```
  git diff --cached
  ```

- **查看两个分支的差异**:

  ```
  git diff <分支1> <分支2>
  ```

### 22. 查看文件状态

- **查看文件的详细状态**:

  ```
  git status -v
  ```

### 23. 查看远程仓库的详细信息

- **查看远程仓库的详细信息**:

  ```
  git remote show origin
  ```

### 24. 查看提交的统计信息

- **查看提交的统计信息**:

  ```
  git log --stat
  ```

### 