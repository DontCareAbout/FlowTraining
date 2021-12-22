score：10 / 100

修正清單：
========

- L1、L2 原本空兩行被刪除
- L4  多了4個 =
- L20 git log -> git 1og
- L31 底線被修改


《我在這個 task 中理解到的 git 是什麼東西》
=======================================

- Git 是一種控制版本的工具，能夠透過將控管資料夾內檔案新增或檔案修改，依照不同時間、作者及檔案紀錄成不同的版本保存下來，因此適合多人團隊共同使用 Git 進行開發 ，同時也可以將檔案還原到不同版本，	此時可以顯示版本間編輯的差異，以利開發者能夠從舊的版本開分支進行開發。
- Git 可以記錄是誰在什麼樣的時間將檔案新增或刪除，透過 Git 進行版本控制，可以釐清任務分工及責任歸屬。
- Git 可以透過 checkout 指令快速的切換版本，並依照開發者需求可以新增 branch 來進行開發，開發完成後再 merge 到另一個 branch 將功能進行整合，而若是有 conflict 時，則需由開發者手動進行選擇版	本。
- commit message 協助開發者能快速知道每個 commit 版本的內容，讓開發者能夠針對需求切換版本，或是對版本進行修改。
- Git 是一款**分散式的版控系統（Distributed Version Control）**，雖然通常也會有共同的伺服器，但即使在沒有伺服器或是沒有網路的環境，依舊可以使用 Git 來進行版控，待伺服器恢復正常運作或是在有網	路的環境後再進行同步，Git 操作也都是在自己電腦本機就可以完成。


Git 指令及說明
--------------

| Git 指令 | 說明 |
| -------- | ---- |
| `git clone` | 將遠端的 repository 下載下來 |
| `git status` | git 目前版本狀態查詢 |
| `git log` | 查看版本歷史紀錄。每個版本上方會寫 commit 後面接一串英數交雜，這個就是版本編號 |
| `git add` | 將所有檔案都加入版本控制（加入資料夾） |
| `git commit` | 建立版本及版本名（命名資料夾名稱） |
| `git checkout` | git checkout + 完整的版本號。將版本更改到版本號的那個版本。 |
| `git branch -v` | 確認主幹及分支 |
| `git branch + 分支名稱` | 新增分支並命名 |
| `git branch –d + 分支名稱` | 刪除分支 |
| `git remote`|  觀看遠端數據庫列表 |
| `git push` | 將本地已經 commit 的版本上傳更新到 github |


 ______________________________________________________________________


## 參考資料 ##

1. [Git 指令](https://hackmd.io/@Yu040419/SyHrpos6V )
2. [Markdown](https://markdown.tw/#hr)
3. [GitHub Docs](
	https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
4. [FlowTraining 中的說明](https://github.com/DontCareAbout/FlowTraining/blob/master/Task_1.md)
