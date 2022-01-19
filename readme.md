# 1.同一文件被提交到本地仓库，pull操作是否覆盖从库本地代码

- 主库操作。修改readme文件，提交到远程main分支
- 从库操作。修改readme文件，提交到远程main分支
- 信息。`failed to push some refs to `
- 需要先使用pull操作将本地代码更新，然后再将代码推到远程main分支
- pull操作后，readme文件产生冲突
- ![image-20220120000444493](readme/image-20220120000444493.png)
- 主从两次操作都显示在文件中，修改文件后，主库提交，从库pull操作同步

# 2.从库文件被修改，但未执行commit等命令，pull操作后，是否会覆盖本地文件-

- 主库push远程仓库
- 从库修改文件，不执行commit命令，直接执行pull命令
- ![image-20220120001904694](readme/image-20220120001904694.png)
- pull操作被终止，需要在merge之前先执行commit或stash命令
- 从库执行git stash命令，控制台信息`Saved working directory and index state WIP on main`
- 从库执行pull操作