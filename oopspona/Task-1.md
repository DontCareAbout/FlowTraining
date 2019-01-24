# Task-1
# 我在這個 task 中理解到的 git 是什麼東西
- Git 是一套分散式的版本控制系統
  - 有了版本控制，不但能輕鬆管理每一個版本的程式碼，還可以將檔案復原到原本的狀態、比對某一段時間的修改
  - 如果要跟多個工程師共同處理一個案子時，不需要帶著隨身碟到處跑來跑去，交換檔案，只需要透過版本控制管理，就能馬上了解對方做了什麼修改
  - 即使在沒有伺服器或是沒有網路的環境，依舊可以使用 Git 來進行版控，待伺服器恢復正常運作或是在有網路的環境後再進行同步，不會受影響
- 免費、開源
  - 除了可免費使用外，整個 Git 的原始程式碼也可在網路上取得（當然 Git 的原始程式碼也是用 Git 在做版本控制的）
- 速度快、檔案體積小
  - Git 特別的設計，在於它並不是記錄版本的差異，而是記錄檔案內容的「快照」（snapshot），它可以讓 Git 在非常快速的切換版本。


## Git 特點
- 可以無窮無盡的開 branch (分支)，好處就是今天不論是修 Bug ，開發新功能，或是研究 feature 都非常的方便
- Git 分為在本地端數據庫操作以及跟遠端數據庫的同步與共享，我們可以在本地端使用像是還原更改等所有Git版本控制功能，但若想要公開本地端的修改內容，或與他人共同修改內容，就必須要透過遠端數據庫的幫忙。

![數據庫](http://www.plantuml.com/plantuml/svg/UpPdpTCv6vwlNlziwevdasSztRNQKTVkPUC2P145AuKdExgUDctMA2Wjpj3aGfFMjNk6QGXOJ_UBFPr0FJavcboOIfoeOOyJcZq0)


## Git 檔案進行版本管理
- 數據庫 : 記錄檔案或目錄狀態的地方，儲存專案的修改歷史記錄，還可以追蹤內容的狀態和版本
- 工作目錄 : 便是我們處理專案的目錄，Git的操作指令都在這裡完成
- 索引 : 為了要將專案上傳到數據庫而準備的暫存區，索引的存在可以排除工作目錄裡不必要的檔案提交，還可以只將檔案變更內容的一部分加入索引並提交。

![檔案版本管理](http://www.plantuml.com/plantuml/svg/UxfzwPEzSvxFNlUofqNNxlcMHK_tJ5MmKdYnOlVJjgud-zSzcxBpwTAzpsUrFDtGyMnXXqPYIeec5qIPhjspgJkUJPxrTDTge8vd_HEUx5hoj6C3N50ZEJytDxD44m00)


## Git 指令的基本用法
- `git clone`： Clone (複製)別人的 Repository
  - 例如我們在 Github 上面看到人家的程式碼想要抓下來自己修改，或是團隊中別人的程式碼，這時候他們通常會有一個 Git 的檔案位置
- `git status`： 在一個 Git 的 Repository 中你可以輸入 git status 來檢查目前 Git 的狀態
- `git log`： 可以使用 git log 的指令查看過去 commit 的紀錄
- `git add`： 新增要讓 Git Repository 被追蹤的檔案
- `git commit`： commit(提交) 紀錄版本變更的摘要
  - 寫程式時一個很重要的動作，一個 commit 在 Git 中就是一個節點，這些 commit 的節點就是未來你可以回朔及追蹤的參考，每一個 commit 就是一次存檔
  - 在 commit 時要清楚表達 commit 的內容
  -  commit 時加上 -m 的參數可快速提交
- `建立 / 切換 branch：git checkout 與 git branch`: 
branch (分支)在一個多人專案的開發過程中我們要開發新功能，修正某個 Bug ，想要測試能不能 work 
  - 我們通常都會從主 branch 再開出一條新的 branch 來做，這支新開的 branch 會帶著你的主 branch 目前的最新狀態，當你完成你所要開發的新功能，Bug 修正後確認沒問題就再把它 merge (合併)回主 Branch ，如此便完成了新功能的開發或是 Bug 的修正
    - git branch ： 這個指令可以列出所有的 branch 並告訴你目前正在哪個 branch
    - git checkout ：切換 branch
- `git remote`: 遠端操作 
- `git push`：在 Git 執行 Push (推送)操作，將本地端的專案上傳


## Git 與 GitHub 

| Git           | GitHub        |
|:-------------:|:-------------:|
| 版本控制系統    | 利用Git進行版本控制，專門用於存放程式碼的共享虛擬主機服務 |


## 參考來源
[Git 的基本使用](https://blog.gogojimmy.net/2012/01/17/how-to-use-git-1-git-basic/)
[學習版本控制基礎](https://windsuzu.github.io/learn-git/)
