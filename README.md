> # 工作流程與作業規範 #


VCS 操作規範
============

我們使用 `git` 作為 VCS、使用 `Github` 作為 VCS host。


Git
---

* 每一個 commit 都要有意義。
* commit message 需要能表現該 commit 的意義
* commit 之間保持「小步前進」的步調


Github
------

以 `FlowTraining` 這個 repo 為例，假設 reviewer 為 `MontyPan`，你（committer）是 `PG`：

    DontCareAbout/FlowTraining -----------------------------------> PG/FlowTraining
               ^                                                           |
               |                                                           |
               +------------------ MontyPan/FlowTraining <-----------------+


PG 的 repo 是由 `DontCareAbout/FlowTraining` fork 出來（等同於 Github 幫你作 `git clone`），
task 完成後發 pull request（簡稱 PR）給 reviewer，
reviewer 如果 accept，就會整合回 `DontCareAbout/FlowTraining`。


### task workflow ###

沿用前述的名詞 / 名稱，假設現在要處理的 task / issue 為 `WtfTask`：

1. 開一個新的 branch，名稱為 `WtfTask`
1. 在 `WtfTask` 上頭作業
1. 完成後發 PR 給 reviewer（`MontyPan/FlowTraining`），
	如果 reviewer 沒有特別指定，target branch 就是 `master`。
1. reviewer 可能會有三個動作：
	* merge pull request：表示 reviewer accept，這個 task 順利結束。
	* comment（包含 line note）：表示 reviewer 認為仍然需要修改、將修改原因與內容寫在 comment 中。
		修改 / commit 完之後，留下一個 comment 通知 reviewer 再次 review。
	* close pull request：表示該 pull request 有重大錯誤，要另外重發 pull request。


另外有幾點注意事項：

* 發 pull request 之後，除非 reviewer 要求修正，否則請不要繼續在該 branch 上 commit。
* 如果該 pull request 在 accept 之前發生 conflict
	（如果發 pull request 的時候還沒有、是 reviewer 後續操作所產生，
	reviewer 有責任寫 comment 通知 committer），
	則此次 pull request 不會被 accept，
	請解決 conflict 之後寫 comment 通知 reviewer。
	解決 conflict 是 committer 的責任，不是 reviewer 的責任。
* 為了防止 dummy 的 merge commit，正常情況下作 `git pull`（或是其他等意指令）時，
	請加上 `--rebase` / `-r` 參數。


文件撰寫規範
============

* UTF-8
* 撰寫中文時請一律使用全形標點符號
* 專有名詞（例如 Java 中的 `class`、`constructor`）一律使用原文
* 中文與英文數字之間用一個半形空白符號隔開。例如：

		我是負責 review 的 reviewer
		
	* 中文標點符號前後的英文數字可省略空白符號。例如：
	
			我是 reviewer，reviewer 負責 review。
		
* 使用 Markdown 語法、搭配 github 延伸語法（[ref.1]、[ref.2]），
	並符合後述的 Markdown Style
    * 若有語法解讀不同的問題，以 GitHub 上能正常顯示為準

[ref.1]: https://guides.github.com/features/mastering-markdown/
[ref.2]: https://help.github.com/articles/github-flavored-markdown/


Markdown Coding Style
---------------------

1. 縮排用 tab
1. header
    1. h1, h2 用 Setext-stye（`====` 與 `----`），要跟 header 一樣長，但不得少於四個。
    1. 除了文件第一行之外，其餘 header 的上頭都要空兩行
		1. 例外：如果連續兩個 header，則 header 之間只要空一行
		1. 例外：作為 blockquote 的 title
	1. header 下頭要空一行
		1. 例外：作為 blockquote 的 title
1. code block
	1. 上頭空一行、下頭空兩行
1. blockquote
	1. 上頭空一行、下頭空兩行
	1. 行首全部都要加上 `>`
	1. 用 blockquote 作諸如「備註」、「注意」的文字區塊，
		則用第六級的 header（稱之為 title），例如：
		
			> ###### title ######
			> 內容內容內容......
1. list
	1. list 區段結束空兩行
	1. list item 的內容超過一行，第二行以後需要縮排
1. horizontal
	1. 上下都要空兩行
	1. 使用 70 個底線
 
			______________________________________________________________________
	
1. link
	1. *建議*使用 reference 方式
	1. reference link 段落上下都要空兩行
1. phrase emphasis 用 `*` 跟 `**` 而不用 `_` 跟 `__`
