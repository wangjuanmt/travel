
## 补充命令
git branch -vv 本地分支和远程分支做跟踪

git checkout src/...  直接抛弃修改

git reset   返回到最新的commit之前，修改的文件保留
git reset --hard  返回到最新的commit之前，修改的文件不保留

git stash 把当前文件存到暂存区

git stash pop 为了fix 一个紧急的bug,  先stash, 使返回到自己上一个commit, 改完bug之后再stash pop, 继续原来的工作。

git commit -a -m "" add and commit

git diff a b 与 git diff b a 方向性

git diff master..test
上面这条命令只显示两个分支间的差异，如果你想找出‘master’,‘test’的共有 父分支和'test'分支之间的差异，你用3个‘.'来取代前面的两个'.' 。

git diff master...test

## .git的密码
cd .git

vim HEAD   内容是ref

cd ref/tags  里面是本地所有的tag

每一个tag就是一个commit 

用tag发布，就是把HEAD指向tag



