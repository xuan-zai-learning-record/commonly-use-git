### 在这里记录一些常用的 git 指令

1. 将远程的代码仓库复制到自己的本机中
    ```
    git clone [url:然后这里填入远程仓库的地址]

    // 如：git clone git@github.com:xuan-zai-learning-record/commonly-use-git.git
    ```

2. 暂存你修改的文件到工作区
    - 暂存单个文件
    ```
    git add [file]
    // 如：git add readme.md  这样只能将 readme.md 进行暂存
    ```
    - 暂存所有文件
    ```
    git add .
    ```
    - 暂存已经跟踪的文件
    ```
    git add -u
    ```
3. 将暂存中的文件保存到本地仓库中
    ```
    git commit -m '在这里填写本次修改的介绍'
    // 如：git -m ':new: 建立了一个用于存放 git 常用命令的仓库'
    ```
4. 查看本地仓库中文件的状态
    ```
    git status
    ```
5. 提交本地仓库到远程仓库
    ```
    git push origin [分支名]
    // 如： git push origin master
    ```
6. 切换分支
    ```
    git checkout [分支名]
    // 如：git checkout dev
    ```
7. 创建分支
    ```
    git branch [分支名]
    // 如： git branch dev
    ```
8. 查看所有的分支
    ```
    git branch -a
    ```
9. 查看所有的提交记录
    ```
    git log
    ```
10. 取消本次的提交，并且保留工作区中的更改
    ```
    git reset --soft [提交的记录 id]
    // --soft: 只删除commit，但不删除实际更改，将更改放入暂存区
    ```
11. 拉去远程仓库最新的代码到本地仓库中
    ```
    git pull
    ```
12. 创建一个新的分支并且切换到该分支中
    ```
    git checkout -b [分支名]
    ```