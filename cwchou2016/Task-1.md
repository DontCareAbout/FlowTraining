我在這個 task 中理解到的 git 是什麼東西
===================================

* git 為版本控制的軟體，方便追蹤變更的內容。一般常用於程式開發。
* 當檔案內容改變時，會跟上一個版本進行比較，並標示出差異的部分。
* 可在不同版本間任意轉換。
* 可用於追蹤所有類型的檔案，但是只有純文字檔才能與不同版本比較。


### 常用 git 指令 ###

* `git clone`：下載網路上的 repo
* `git status`：查看目前版本修改的檔案
* `git log`：查看過去 commit 的紀錄
* `git add`：新增要被追蹤的檔案
* `git commit`：紀錄版本變更的摘要
    * 每個 commit 的紀錄訊息都有要意義
    * `git commit -m "<message>"` 可快速 commit
* `git branch`：查看、建立或刪除 branch
	* `git branch <新 branch 名稱>`
	* `git branch -d <要刪除的 branch>`
* `git checkout`：切換 branch
* `git remote`：管理遠端的 repo
* `git push`：將整個 repo 上傳


### Markdown Software ###

|Software   |OS     |Download                         |
|:----------|:------|:--------------------------------|
|MarkdownPad|Windows|[link][MP]                       |
|Retext     |Linux  |Ubuntu: `sudo apt install retext`|

[Others](https://itsfoss.com/best-markdown-editors-linux/)

[MP]:http://markdownpad.com/


###參考連結###

1. [Git-Tutorials](https://github.com/twtrubiks/Git-Tutorials)
2. [工作流程與規範](https://github.com/DontCareAbout/FlowTraining/blob/master/README.md)  
