score: 15/100


修正清單：
==========

* L6 把 Git**h**ub 改成 Git**H**ub -> 英文字母小寫改大寫
* List 最後一項新增「遠端檔案庫（remote repo）
* L18 新增一行空行
* L22 3**O**00 改成 3**0**00 -> 英文字母改成數字
* L24 loca**1** 改成 loca**l** -> 數字改成英文字母

______________________________________________________________________


《我在這個 task 中理解到的 Git 是什麼東西》
=====================================

Git 是一種方便回顧過往版本的版本控制系統，把檔案修改完成要 commit 時可以留下 message 紀錄，以供每個之後要瀏覽版本資訊的人參考。

Git 可以使用指令跟 GitHub 連結，像是可以把 GitHub 的遠端檔案庫中的專案複製到本地端檔案庫，或是把本地端檔案庫的檔案上傳到 GitHub 的遠端檔案庫。

Git 在紀錄更新的檔案時，只會記錄有變動的資訊，所以在 push 至 GitHub 後，在 GitHub 的新版本更新檔也只會顯示有修改的部分。


* 環境
	* local（本地端）
		* 專案資料夾（working directory）
		* 暫存區（staging area）
		* 本地檔案庫（local repo）
	* remote（遠端）
		* 遠端檔案庫（remote repo）



> ###### 舉例來說 ######
> A 君＆B 君＆C 君需要一同拚一個 3000 片的拼圖，他們分別被分配了須完成左、中、右三個區塊，
> 在工作期間他們可以各自做自己的部分，首先他們需要各自先找一個合適的地方（working directory）並會在此作業，
> 當他們將自己的完成品集中（staging area）並確認沒問題後，放入（commit）各自的固定邊框（local repo），
> 最後放上（push）完成品集中區（remote repo） 。




Git 指令
--------

| 指令                    | 說明                                                                      |
|-------------------------|---------------------------------------------------------------------------|
| git clone  <url>        | 將網路上的 repository 遠端下載至本地電腦（建議用 clone with HTTPS）|
| git init                | 初始化專案並會產生 .git 的資料夾（為隱藏的狀態）|
| git add .               | 將工作資料夾全部檔案加入暫存區（staging area）並開始被追蹤|
|                         | （需要先將工作資料夾初始化並產生 .git 這個儲存版本的資料夾）
| git add <檔案名稱>      | 指定某個檔案加入暫存區|
|                         |（需要先將工作資料夾初始化並產生 .git 這個儲存版本的資料夾）|
| git status              | 查詢這個資料夾內的狀態（需先加到暫存區）|
|                         | 未被列入被追蹤的檔案會顯示 untracked| 
| git branch              | 查看全部分支|
| git branch <名稱A>      | 建立名為 "名稱A" 的分支 |
| git checkout <名稱A>    | 切換至 "名稱A" 分支|
| git commit -m "敘述原因"| 提交至本地檔案庫|
|                         | 若尚未設定過帳戶，提交前會需要設定 email 和 name|
| git push                | 上傳至遠端檔案庫（例如：GitHub）|
| git pull                | 下載至本地檔案庫 |
| git log                 | 顯示提交歷史紀錄 |
| git remote              | 檢視所有已經設定好的遠端檔案庫 |


參考資料
-------

1. [Git 安裝教學](https://progressbar.tw/posts/1 " Git 安裝教學")
2. [GitHub 首頁](https://github.com/ "GitHub 首頁")
3. [Markdown 線上編輯器](https://hackmd.io/ " Markdown 線上編輯器")