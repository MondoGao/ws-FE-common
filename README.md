# WESharp 前端组共用仓库
## 分支管理
- 各成员禁止在 master 分支上进行 merge 操作，只能从自有分支 merge master 分支
- 建立个人分支，分支命名格式为 member/[name]，如 member/mondo
- 可在本地仓库建立其他分支，但只推送上述个人主分支，推荐分支如下：
    - [name]/dev 测试环境分支
    - [name]/feature 新功能分支
    - [name]/hotfix 修复 bug 分支
- 为防止误操作，请在仓库主目录下新建以 name 为名的文件夹，在该文件夹中进行开发，如
    
    ```bash
    # 位于 member/mondo 下
    - we-FE-common （仓库主文件夹）
        |- .gitignore
        |- README.md
        |- ... （master 分支上的其他通知、任务文件（夹））
        |- mondo （个人文件夹）
            |- task1 （项目文件夹/子项目）
                |- README.md
            |- task2
            |- ...
    ```
    
    > task1，task2 等任务文件夹可使用 git 子项目进行管理
    
## 注意事项
1. 开会前 push 自己的分支到服务器上
2. 子项目可以是公开（public）项目，具体操作请自行百度
3. 分支 merge 可按自行喜好保留分支记录（使用 --no-ff 命令）
4. 每个任务下必须有 README.md，内容为项目心得、更新记录及其他信息