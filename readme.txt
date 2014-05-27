Git 版本库的学习
这是学习过程中的测试文件。
时光机穿梭：
修改一下这个文件。
版本回退。
总结一下，目前学到的命令有：
git add
git commit
git status
git diff
git log
git relog
git reset --hard
继续，工作区和暂存区的学习
再做一个修改
再来一个
再总结一下：
工作区内容修改的回退：git checkout -- readme.txt
已加入暂存区的内容修改回退需要先：git reset HEAD readme.txt,再进行上面的工作区撤销
已经提交了的只能进行版本回退了
同步到github远程库，先总结下：
 git remote add origin https://github.com/amoy0226/git_study.git进行关联
 git push -u origin master进行第一次推送master分支到远程库
 git push origin master以后本地提交后，使用这个命令更新到远程库
从github远程库克隆到本地，总结下：
 github创建远程库gybzpxt
 git bash定位到本地目录，使用git clone git@github.com:amoy0226/gybzpxt.git命令克隆到本地
 会在本地生成gybzpxt目录，同步成功
<<<<<<< HEAD
<<<<<<< HEAD
 这是master分支
=======
 git checkout -b dev增加并切换到dev分支
>>>>>>> dev
=======
 这是master分支
 快进模式合并分支
>>>>>>> dev
快进模式合并分支dev1
<<<<<<< HEAD
master分支中添加的修改
=======
增加新分支feature1
>>>>>>> feature1
分支合并
创建并切换dev分支
dev分支的工作进行到一半，master上有个bug要修复
做个总结吧：
	git branch 用于新建分支（-d删除，-D强制删除）
	git checkout 用于切换分支
	git merge 将指定分支合并到当前分支
	git metge --no-ff -m "说明" dev 合并分支，并不采取fast forward模式
	git stash 用于暂时保存工作现场
	git stash list 显示暂存的工作现场
	git stash apply stash@{stashnumber} 来恢复现场
	git stash drop 删除现场
	bug修复，功能增加都应该通过新建分支来完成，然后再合并
<<<<<<< HEAD
shrimp对dev分支进行了修改
=======
otherpeople对dev分支进行了修改
>>>>>>> cbafdb574bfc2e26809bedff75ea21fc9ce6e1e7
解决冲突