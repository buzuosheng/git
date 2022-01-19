# 1.单个文件修改，pull操作是否修改本地代码

- 主库操作。修改readme文件，提交到远程main分支
- 从库操作。修改readme文件，提交到远程main分支
- 信息。`failed to push some refs to `
- 需要先使用pull操作将本地代码更新，然后再将代码推到远程main分支
- pull操作后，readme文件产生冲突
- ![image-20220120000444493](readme/image-20220120000444493.png)
- 主从两次操作都显示在文件中，修改文件后，主库提交，从库pull操作同步

