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
修复bug
学了标签的使用，总结下：
	git tag tagname 创建标签
	git tag tagname logid 创建指定提交上的标签
	git tag -d tagname 删除本地标签
	git push origin :refs/tags/taaname 删除远程库标签
	git push origin tagname 提交标签到远程库
	git push origin --tags 提交所有未提交标签
	