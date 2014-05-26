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
 