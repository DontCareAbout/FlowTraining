> # 《我在這個 task 中理解到的 git 是什麼東西》 #
> * 作業日期：2018/10/23
> * 學生：SeanWalk
> * 版本：1.0.2


git 在做什麼
------------
Git 是一個開源的分佈式版本控制系統，可以有效、高速的處理從很小到非常大的項目版本管理。而分佈式相比於集中式的最大區別在於開發者可以提交到本地，每個開發者通過 `git clone`，在本地機器上 copy 一個完整的 Git repository。一個正確的 Git 開發過程如下。
1. 從伺服器上 clone 完整的 Git repository (包含程式碼與版本號)到本地主機上。
1. 在本地主機上根據不同的開發目的，創建 branch，修改程式碼。
1. 在本地主機自己創建的 branch 上做 commit。
1. 在本地主機上合併　branch。
1. 把 Server 上最新版的程式碼 fetch 下來，與自己的合併。
1. task 完成後發 pull request 給 reviewer， reviewer 如果 accept，就會整合回 master


git 指令簡介
------------

| Command | Description |
| --- | --- |
| `git clone` | Cloning an Existing Repository |
| `git status` | Checking the Status of Your Files |
| `git log` | Show commit logs |
| `git add` | Staging Modified Files |
| `git commit` | Committing Your Changes |
| `git branch` | Make a branch |
| `git checkout` | Move to another branch |
| `git remote` | Manage set of tracked repositories |
| `git push` | Update remote refs along with associated objects |


參考資料
-------
1. [Markdown table][table]
1. [git 指令說明][git command]
1. [百度 git 簡介][baidu git]
1. [Flow參考][Flow]


[table]: https://help.github.com/articles/organizing-information-with-tables/
[git command]: https://git-scm.com/doc
[baidu git]: https://baike.baidu.com/item/Git/12647237#1
[Flow]: https://github.com/DontCareAbout/FlowTraining

