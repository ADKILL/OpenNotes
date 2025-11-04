<!--
本文归属项目：`OpenNotes`
本文修订状态：初稿 20250922
-->


# Git 常用操作命令及作用

本文总结了 Git 的常用命令及其对应作用，便于快速查询和学习。

---

## 一、Git 基础配置

| 命令 | 作用 |
|------|------|
| `git config --global user.name "用户名"` | 设置全局用户名 |
| `git config --global user.email "邮箱"` | 设置全局邮箱 |
| `git config --list` | 查看当前配置 |
| `git help <command>` | 查看某个命令的帮助 |

---

## 二、仓库初始化与克隆

| 命令 | 作用 |
|------|------|
| `git init` | 初始化一个新的 Git 仓库 |
| `git clone <url>` | 克隆远程仓库到本地 |
| `git clone -b <branch> <url>` | 克隆远程仓库并切换到指定分支 |

---

## 三、文件操作

| 命令 | 作用 |
|------|------|
| `git status` | 查看当前仓库状态 |
| `git add <file>` | 将指定文件添加到暂存区 |
| `git add .` | 将所有修改文件添加到暂存区 |
| `git rm <file>` | 删除文件并从 Git 中移除 |
| `git mv <old> <new>` | 重命名文件 |

---

## 四、提交记录

| 命令 | 作用 |
|------|------|
| `git commit -m "说明"` | 提交暂存区的内容 |
| `git commit -am "说明"` | 跳过 `git add`，直接提交已跟踪文件 |
| `git log` | 查看提交历史 |
| `git log --oneline --graph --all` | 图形化查看分支历史 |

---

## 五、分支管理

| 命令 | 作用 |
|------|------|
| `git branch` | 查看本地分支 |
| `git branch <name>` | 创建新分支 |
| `git checkout <name>` | 切换到指定分支 |
| `git checkout -b <name>` | 创建并切换到新分支 |
| `git merge <branch>` | 合并分支到当前分支 |
| `git branch -d <name>` | 删除分支 |
| `git switch <branch>` | 新版切换分支 |
| `git switch -c <branch>` | 新版创建并切换分支 |

---

## 六、远程仓库操作

| 命令 | 作用 |
|------|------|
| `git remote -v` | 查看远程仓库信息 |
| `git remote add origin <url>` | 添加远程仓库 |
| `git remote remove origin` | 移除远程仓库 |
| `git fetch origin` | 从远程获取最新数据 |
| `git pull origin <branch>` | 拉取远程分支并合并 |
| `git push origin <branch>` | 推送本地分支到远程 |

---

## 七、撤销与回滚

| 命令 | 作用 |
|------|------|
| `git checkout -- <file>` | 撤销工作区修改 |
| `git reset HEAD <file>` | 取消暂存区的文件 |
| `git reset --hard <commit>` | 回滚到指定提交（丢失修改） |
| `git revert <commit>` | 撤销指定提交（保留历史） |
| `git clean -fd` | 删除未跟踪文件和目录 |

---

## 八、标签管理

| 命令 | 作用 |
|------|------|
| `git tag` | 查看标签 |
| `git tag <name>` | 创建轻量标签 |
| `git tag -a <name> -m "说明"` | 创建带说明的标签 |
| `git push origin <tag>` | 推送标签到远程 |
| `git push origin --tags` | 推送所有标签 |

---

## 九、暂存与恢复

| 命令 | 作用 |
|------|------|
| `git stash` | 暂存当前工作区修改 |
| `git stash list` | 查看暂存记录 |
| `git stash apply` | 恢复暂存但保留记录 |
| `git stash pop` | 恢复暂存并删除记录 |

---

## 十、其他常用命令

| 命令 | 作用 |
|------|------|
| `git diff` | 查看修改内容 |
| `git diff --cached` | 查看暂存区与最新提交的差异 |
| `git blame <file>` | 查看文件每行的提交历史 |
| `git show <commit>` | 查看某次提交的详细信息 |

---

📌 **提示**  
- 常用流程：`git init` → `git add` → `git commit` → `git push`  
- 推荐使用 `git log --oneline --graph --all` 清晰查看分支历史。

