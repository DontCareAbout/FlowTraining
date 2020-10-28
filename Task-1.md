《我在這個 task 中理解到的 git 是什麼東西》
=====================================

git 是一種 [VCS(Version control system)](https://zh.wikipedia.org/wiki/Subversion)。  
當程式碼修改完成而 commit 時，git 會生成一個 version。透過 git log 可以方便並快速的瞭解每個版本修改的原因。當新版本出現問題，透過 git diff 可方便比對不同版本間的差異。如果需要更可快速切換回上一版本的程式碼。  

在同時多人開發多個功能時，透過 branch 與 merge 可讓彼此之間的程式碼不互相干擾。
git 的 log 會在本地端儲存一份與 Server 處於離線狀況，對於不在同一地點或時間開發的人員，在檢查 log 與 commit 時更加方便。  

### git 與 svn 部份指令的對照 ###
git 指令 | 作用 | svn 指令 |
--------|---------|-----|
clone | 下載一份程式碼至本地目錄 | checkout (co) |
status | 查看修改的檔案 | status
log | 查看過去的修改記錄 | log
add | 新增要被追蹤的檔案 | add
commit | 將修改內容記錄在本地 repository |      |
remote | 維護遠端檔案 |  |
push | 將修改的內容更新至伺服器 | commit |
checkout | 切換至不同的 branch | switch |
branch | 建立一個 branch | copy |
pull | 更新伺服器上的最新版本或特地版本至本地 | update |

### Reference ###
* [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
* [SVN 基本指令教學](https://blog.longwin.com.tw/2007/07/svn_tutorial_2007/)
* [Git 初學筆記](https://blog.longwin.com.tw/2009/05/git-learn-initial-command-2009/)
