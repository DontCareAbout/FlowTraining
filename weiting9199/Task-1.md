0/100


被亂改的修正清單
----------------

* 原 L01：「到」被刪掉
* 原 L06：「會」被刪掉
* 原 L08：多「全」
* 原 L19：多一個 tab
* 原 L27：字母「l」被改成數字「1」
* 原 L36：被刪掉
* 原 L60、L61：網址前面多一個空格


我在這個 task 中理解到的 git 是什麼東西
=====================================

* 分散式版本控制軟體（去中心化版本控制軟體）
	* 我對去中心化的理解是因為比特幣（暴漲那時候有稍微去了解）
	* 看過一個比喻是說「村子裡的大家都會有一本帳本，用於紀錄村子的公共資產，只要有人在帳本上更改，
		就會用廣播器讓全村的人知道，於是全村的人都會將廣播器的內容記錄在自己的帳本上」
		* 若要竄改帳本，就要把全村的人的帳本都改過
		* 相反的比喻就是「紀錄村子公共資產的帳本只有村長有，其他人都沒有」
	* 透過這個理解，我把 Repository 視為帳本
* 方便程式設計師可以一起修改同一個 Repository 的內容
	* 會記錄每個人的修改紀錄（帳本）
	* Repository
		1. 延伸出新點子（branch）：也許是為了精簡，也許是為了測試，而延伸出不同的寫法
		2. 隨時可以找到紀錄點（節點）
		3. 不會忘記主線（master）：同 a 點，如果沒有 master 可能寫著寫著就忘記自己原本的想法
			* 我的意思是，在不刪掉他的前提下，因為今天要做一個東西，應該不會輕易改變目標的
			* 我認為刪掉的情況可能是覺得這個延伸的新點子不好
			（為了完成一個目標可以有多個方法，一開始寫 a ，後來發現 b 方法更精簡、有效率，於是捨棄 b 方法）


指令
----

### repository（倉儲） ###

* `git clone [url]`：將網路上的 Repository 下載至本地電腦
* `git init`：初始化（建立 `.git` 的子資料夾）


### branch（分支） ###

* `git branch`：查看所有 branch
	* `git branch <new_branchname>`：建立新的 branch 並命名
	* `git branch -m <original_branchname> <new_branchname>`：重新命名 branch
	* `git branch -d <branchname>：刪除指定的 branch
* `git checkout <branchname>`：切換至指定 branch（預設為 `master`）
	* `git checkout -b <branchname>`：建立並切換至指定 branch
	* `git diff <branchname1> <branchname2>`：比較兩個 branch 的不同之處


### commit（提交） ###

* `git status`：查看狀態
* `git add <filename>`：將檔案從 Working Directory 移至 Staging Area（commit 的前置作業）
* `git commit -m "<此次修改的內容>`：將檔案從 Staging Area 提交至 Repository（快速提交）
	* `git commit -a -m "<此次修改的內容>"`：`git add` 並快速提交（之前沒有 add 過的不適用）
* `git log`：查看 commit 的紀錄


Git 與 GitHub
-------------

| Git   | GitHub |
| ----- | ------ |
| 軟體   | 網站   |
| [link][Git]| [link][GitHub]|


[Git]:https://git-scm.com/
[GitHub]:https://github.com/

