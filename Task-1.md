《我在這個 task 中理解到的 git 是什麼東西》
==========================================

git 是一種分散式的版本控制系統，開發者可以在離線 Local 環境下進行開發，當有網路時再將自己的程式 push 到 Remote 環境或 pull 程式碼給其他開發者進行整合。

* 環境
	* Local (本地)
		* 專案資料夾（Working directory）
		* 暫存區（Staging area）
		* 本地檔案庫（Repository）= Repo
	* Remote (遠端)
	
	
> ###### For example ######
> A君& B君& C君需要一同拚一個3000片的拼圖，他們分別被分配了須完成左、中、右三個區塊，
> 在工作期間他們可以各自做自己的部分，首先他們需要各自先找一個合適的地方（Working directory）並會在此作業，
> 當他們將自己的完成品集中（Staging area）並確認沒問題後，放（commit）入各自的固定邊框（Repository），
> 最後放（push）上完成品集中區（Remote 遠端環境（Github）） 。
		
		
git 指令
---------

| 指令                    | 說明                                                                      |
|-------------------------|---------------------------------------------------------------------------|
| git clone  <url>        | 將網路上的 Repository 遠端下載至本地電腦（建議用 Clone with HTTPS）|
| git init                | 初始化 git 的專案|
| git add .               | 將工作資料夾全部檔案從專案資料夾（Working area）加入暫存區（Staging area）|
| git add <檔案名稱>      | 指定某個檔案從專案資料夾（Working area）加入暫存區（Staging area）|
| git status              | 查詢檔案追蹤的狀態（需先加到暫存區）|
| git branch              | 查看全部分支（branch）|
| git branch <名稱A>      | 建立名為 "名稱A" 的分支 |
| git checkout <名稱A>    | 切換至 "名稱A" 分支|
| git commit -m "敘述原因"| 提交至本地檔案庫|
|                         | 若尚未設定過帳戶，提交前會需要設定 email 和 Name|
| git push                | 上傳至遠端檔案庫（例如：Github）|
| git log                 | 顯示提交歷史紀錄 |
| git remote              | 可以檢視已經設定好的遠端版本庫 |


參考資料
---------

1. [Git 安裝教學](https://progressbar.tw/posts/1 "Git 安裝教學")
2. [Github 首頁](https://github.com/ "Github 首頁")
3. [Markdown 線上編輯器](https://hackmd.io/ "Markdown 線上編輯器")

