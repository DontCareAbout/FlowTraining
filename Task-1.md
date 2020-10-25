《我在這個 task 中理解到的 git 是什麼東西》
=====================================

git 是一種 [VCS(Version control system)](https://zh.wikipedia.org/wiki/Subversion)，跟工作使用的 SVN 使用上最大的不同點是，查 log 超好用。
SVN 查 log 必須與 Server 連線，離線就查不了。SVN 在家要 debug 時超不方便。

### git 與 svn 部份指令的 mapping ###
git 指令 | svn 指令 |
--------|---------|
clone | checkout (co) 
checkout | switch 
branch | copy
push | commit
pull | update

### Reference ###
* [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
* [SVN 基本指令教學](https://blog.longwin.com.tw/2007/07/svn_tutorial_2007/)
* [Git 初學筆記](https://blog.longwin.com.tw/2009/05/git-learn-initial-command-2009/)
