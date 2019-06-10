# 我在這個 task 中理解到的 git 是什麼東西

-  分散式版本控制軟體
-  可以分成三個區塊
   1. 工作目錄（Working Directory）
   2. 暫存區（Staging Area）
   3. 儲存庫（Repository）
## 指令
### directory（目錄）
- `pwd`：查看目前所在的目錄
- `ls`：查看目錄中的檔案
- `cd`：變更目錄
  - `cd <directoryname>`：前往下一層目錄
  - `cd ..`：返回上一層目錄
  - `cd ~`：返回初始目錄
### repository（倉儲）
- `git clone [url]`：將網路上的 repo 下載至本地電腦
- `git init`：初始化（建立`.git`的子資料夾）
### branch（分支）
- `git branch`：查看所有 branch
  - `git branch <new_branchname>`：建立新的 branch 並命名
  - `git branch -m <original_branchname> <new_branchname>`：重新命名 branch
  - `git branch -d <branchname>`：刪除指定的 branch
- `git checkout <branchname>`：切換至指定 branch（預設為 `master`）
  - `git checkout -b <branchname>`：建立並切換至指定 branch
  - `git diff <branchname1> <branchname2>`：比較兩個 branch 的不同之處