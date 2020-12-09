#### 常用Git命令

| 命令                     | 作用                                           |
| ------------------------ | ---------------------------------------------- |
| git init                 | 初始化，创建 git 仓库                      |
| git status               | 查看 git 状态 （文件是否进行了添加、提交操作） |
| git add 文件名           | 添加，将指定文件添加到暂存区                  |
| git commit -m '提交信息' | 提交，将暂存区文件提交到历史仓库               |
| git log                  | 查看日志（ git 提交的历史日志）              |




#### 版本控制常用命令

| 命令                            | 作用                                                         |
| ------------------------------- | ------------------------------------------------------------ |
| git reflog                      | 可以查看所有分支的所有操作记录（包括已经被删除的 commit 记录的操作） |
| git reset --hard 版本唯一索引值 | 将库修改到指定版本                                           |



#### 分支管理常用命令

| 命令              | 作用     |
| --------- | -------- |
| git branch 分支名 | 创建分支 |
| git checkout 分支名 | 切换分支 |
| ls | 查看文件命令 |
| git merge 分支名 | 合并分支 |
| git branch -d 分支名 | 删除分支 |
| git branch | 查看命令 |



#### 远程仓库相关命令

- 首先要生成SSH公钥

  设置Git账户

  + git config user.name（查看git账户）
  + git config user.email（查看git邮箱）
  + git config --global user.name “账户名”（设置全局账户名）
  + git config --global user.email “邮箱”（设置全局邮箱）
  + cd ~/.ssh（查看是否生成过SSH公钥）

  生成SSH公钥

  + 生成命令: ssh-keygen –t rsa –C “邮箱” ( 注意：这里需要敲3次回车)

  查看命令: cat ~/.ssh/id-rsa.pub

  在gitee或者github上设置公钥

  公钥测试

  + 命令: ssh -T git@gitee.com

-  推送到远程仓库

  - 为远程仓库的URL，自定义仓库名称

    git remote add 远程名称 远程仓库URL

  - 推送

    git push -u 仓库名称 分支名

##### 当本地没有仓库，从远程拉取

1. 将远程仓库的代码，克隆到本地仓库
   克隆命令：git clone 仓库地址
2. 创建新文件，添加并提交到本地仓库
3. 推送至远程仓库
4. 项目拉取更新
   拉取命令：git pull 远程仓库名 分支名