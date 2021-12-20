

《我在這個 task 中理解到的 git 是什麼東西》
=======================================

- Git 是一種控制版本的工具，能夠透過將控管資料夾內檔案新增或檔案修改，依照不同時間、作者及檔案紀錄成不同的版本保存下來，因此適合多人團隊共同使用 Git 進行開發 ，同時也可以將檔案還原到不同版本，	此時可以顯示版本間編輯的差異，以利開發者能夠從舊的版本開分支進行開發。
- Git 可以記錄是誰在什麼樣的時間將檔案新增或刪除，透過 Git 進行版本控制，可以釐清任務分工及責任歸屬。
- Git 可以透過 checkout 指令快速的切換版本，並依照開發者需求可以新增 branch 來進行開發，開發完成後再 merge 到另一個 branch 將功能進行整合，而若是有 conflict 時，則需由開發者手動進行選擇版	本。
- commit message 協助開發者能快速知道每個 commit 版本的內容，讓開發者能夠針對需求切換版本，或是對版本進行修改。
- Git 是一款**分散式的版控系統（Distributed Version Control）**，雖然通常也會有共同的伺服器，但即使在沒有伺服器或是沒有網路的環境，依舊可以使用 Git 來進行版控，待伺服器恢復正常運作或是在有網	路的環境後再進行同步，Git 操作也都是在自己電腦本機就可以完成。


GitHub flow
-----------

###### 建立 Branch ######
> GitHub Flow 是一個基於分支（Branch）的輕量化工作流程，幫助團隊及專案定期的進行部署。
> GitHub Flow 只需要記住主分支 master 其他分支都是從主分支在開出來，不管是解 Issue 還是開發新功能，都是以 master 分支為基底來建立新的分支
> 當在進行一個功能開發或修復時，分離出新分支與 master 是非常重要的。分支命名應該具有描述性（如 refactor-authentication、user-content-cache-key 或是 make-retina-avatars），讓其他人清楚知道> 分支正在進行的工作項目。


###### 新增 Commit ######
> 建立 Branch 後，可以新增、修改、刪除檔案，並提交更新且將檔案加入分支，每個提交都會有相關的提交訊息，可以讓其他人了解工作紀錄並提供回饋，同時也可以在找到錯誤或是修正方向時可以復原修改。


###### 開啟 Pull Requst ######
> Pull Request 是關於提交（Commit）的討論。可以在開發過程任何時間點，開啟一個 Pull Request，比如準備好讓專案維護者檢閱工作項目時，可以使用 Pull Request 的訊息與團隊成員討論。
> Pull Request 用於協作開源專案和管理共享儲存庫的修改，Pull Request 提供了一個方式來通知專案維護者來考慮使用所做的修改。


###### 討論與檢閱程式碼 ######
> Pull request 的評論主要用 Markdown 撰寫，檢閱修改的人或維護團隊可能會提出問題或意見。也許是程式碼風格不符合專案規範、缺少單元測試，或者也許一切看起來都不錯且狀況良好。Pull Request 旨在鼓勵> 這種類型的討論。
> 在討論及回饋關於提交時，可以繼續 Push 到你的分支。如果團隊成員反應說你忘了做某件事，或者在程式碼中有錯誤，你可以在分支中修正它並繼續推送修改。


###### 部屬 Deploy ######
> Pull Request 已經被檢閱且分支通過測試，假如你的分支產生問題，可以重新部署 master 復原。


###### 合併 Merge ######
> Merge 之後，Pull Request 保存了一筆程式碼的修改歷史記錄，可讓任何人回頭來了解為什麼及如何作出決定。



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
5. [GitHub Flow](https://medium.com/@trylovetom/%E8%AE%93%E6%88%91%E5%80%91%E4%BE%86%E4%BA%86%E8%A7%A3-github-flow-%E5%90%A7-4144caf1f1bf)
