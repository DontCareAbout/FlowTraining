> # Task 2 #
> * 項目：git pull
> * 完成條件：pull request accept


瞭解 `git pull` 的意義與操作方式。

大多數情況下我們都會搭配 `-r` 這個參數使用，以避免無謂的 merge commit。


Task Feedback
=============
 
1. 使用 `git pull -r` 將自己 local repo 的 master branch 與 `DontCareAbout` repo 的 `master` 一致
1. 使用 `git push` 讓自己的 github repo 的 master branch 與 `DontCareAbout` repo 的 `master` 一致
1. 建立一個 branch，名稱為 `task-2`，並切換到這個 branch
1. 修正被亂改 `Task-1.md`（會放在以你 GitHub 帳號名稱命名的目錄下），並在結尾加上 Task-1 的分數
	* Task-1 的分數在 merge 的 commit log 中
1. 發 pull request 給 `MontyPan/FlowTraining` 的 `master`

注意：如果沒有使用 `-r` 導致出現 merge commit，則 pull request 必定會 reject
