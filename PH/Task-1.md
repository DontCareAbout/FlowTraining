# 我在這個 task 中理解到的 git 是什麼東西

 1. 一套版本控制系統。目前看起來，是個能夠紀錄文件更動版本（含作者、時間），同時複合協作並比對出資料更動部份。
 2. GitHub 為使用 git 的平台之一。
 3. 每個人可以透過 git 將 GitHub 上的資料現有版本下載至本地資料夾，並進行更動後上傳更新。
 
 
## 目前理解的 git 操作

#### 1. 透過 fork 將 GitHub 上的資料（FlowTraining）複製一份，加進自己的 repository 中進行檔案內容更動或是檔案增刪。

    Note. 若是沒先 fork 到自己的 repository，直接進行下列操作，應該不會影響原作者的檔案，但也無法進行協作或增刪？
 
 
 
#### 2. 針對剛加至 repository 的資料 clone 到本地資料夾（A）中。
 透過命令提示字元進入 A 資料夾，將 FlowTraining 的 SSH clone 到資料夾中
 
> git clone git@github.com:49831117/FlowTraining.git
 
#### 3. 進行資料更動。

 有使用到的 cmd 輸入指令 | 使用指令的回饋
 --- | --- 
 git status | 目前資料夾中的狀態，包含有無更動、有無暫存檔。<br>以本次操作為例，將 task-1/Task-1.md 移入 FlowTraining 後，<br>會看到 <code>Untracked files:</code> 出現紅色的 <code>task-1/</code></br>
 git add task-1/ | 將 task-1/ 加入暫存檔
 git commit -m "增加task-1/Task-1.md" | 紀錄更動以及更動的註解
 git push | 將更動推上 GitHub
 git help | 搭配 [Google](https://www.google.com/") 解惑用

    Note. 操作 git push 的過程中曾遇過反饋是 Everything up-to-date，但 GitHub 上卻沒更新？
    （Google 到的解決方法是透過 newbrench，但仍舊沒上傳成功）


## 簡單心得

過去曾經負責過跨部門（？）合作的計畫，過程中的每次討論、預算控管其實都需要留下修正紀錄，
常常 Word 存了好幾個版本、Excel 開了數個分頁來紀錄版本差異。雖然尋找過去版本資料時都有紀錄，
但仍然無法滿足部門間資料同步、銜接的需求，而 git 目前看起來是能解決這部份問題的解法。
