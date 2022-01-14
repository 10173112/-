

## Git- 取消commit五. 將commit拆掉●新增檔案：vi hello.py●將檔案加入索引：$ git add .●提交版本：$ git commit -m “print method”●查看歷史紀錄：$ git log●取消commit：$ git reset --mixed HEAD^●查看歷史紀錄：$ git log●查看狀態：$ git status#  ^ 符號表示「前一次」的意思，回到前n個HEAD~nLocal(本地端)#  會發現最後一次commit的紀錄不見了#  會出現hello.py尚未被追蹤，代表此時檔案在工作目錄
## Git- Reset模式--mixed--soft--hardcommit拆出來的檔案丟回工作目錄丟回暫存區直接丟掉Reset有三種模式：●--mixed：預設模式，Commit 拆出來的檔案會留在工作目錄，但不會留在暫存區●--soft：工作目錄跟暫存區的檔案都不會被丟掉●--hard：工作目錄以及暫存區的檔案都會丟掉
## Git-使用方法六.
進入Remote repository(遠端數據庫)1.雲端跟本地端連動：$ git remote add origin <remote網址>2.Push Local master(主幹)進入Remote：$ git push --set-upstream origin master3.回到Github查看10Remote(雲端)＃等同於$ git push -u origin master＃-u : 設定要push到哪裡，當之後push不加參數時，會將本地Local repo的master分支，push到遠端的origin節點下
## Git-使用方法七.
Remote repository(遠端數據庫)1.到github上新增或編輯README.md2.把遠端東西拉回來：$ git fetch3.查看狀態：$ git status4.查看歷史紀錄：$ git log5.比較本地分支和遠端分之內容的不同：$ git diff origin/master6.將遠端和本地端的內容做合併：$ git merge origin/master7.查看狀態：$ git status8.Pull下載更新：$ git pull origin11Remote(雲端)# 將本地master的資料更新, 以防與Remote端不同# 執行Fetch 指令後，Git 看了一下線上版本的內容後，將目前線上有但本地這邊沒有的內容抓了一份下來# 會發現在github上發送的commit被抓下來了
## 什麼是Git Flow？
## Git Flow分支應用●主要的分支有master、develop、hotfix、release以及feature●各種分支負責不同的功能●Master以及Develop這兩個分支又被稱做長期分支，會一直存活在整個Git Flow 裡●其它的分支大多會因任務結束而被刪除
## Git Flow分支應用●Master 分支○主要是用來放穩定、隨時可上線的版本。○這個分支的來源只能從別的分支合併過來○通常會在這個分支上的Commit 上打上版本號標籤。●Develop 分支○所有開發的基礎分支○當要新增功能的時候，所有的Feature 分支都是從這個分支切出去的。而功能完成後，也都會合併回來這個分支。

## Git Flow分支應用●Hotfix 分支○當線上產品發生緊急問題的時候，會從Master 分支開一個Hotfix 分支出來進行修復，Hotfix 分支修復完成之後，會合併回Master 分支，也同時會合併一份到Develop 分支。●Release 分支○當認為Develop 分支夠成熟了，就會合併到Release 分支，在這邊進行上線前的最後測試。○測試完成後，Release 分支將會同時合併到Master 以及Develop 這兩個分支上

## Hotfix 分支○當線上產品發生緊急問題的時候，會從Master 分支開一個Hotfix 分支出來進行修復，Hotfix 分支修復完成之後，會合併回Master 分支，也同時會合併一份到Develop 分支。●Release 分支○當認為Develop 分支夠成熟了，就會合併到Release 分支，在這邊進行上線前的最後測試。○測試完成後，Release 分支將會同時合併到Master 以及Develop 這兩個分支上
## Git Flow分支應用●Feature 分支○當要開始新增功能的時候○從Develop 分支來的，完成之後再併回Develop 分支。
## 什麼是虛擬機？●行為類似 實際電腦 的電腦 檔案(通常稱作 映像)。●可在視窗中 以獨立的運算環境 執行●常用來執行不同的作業系統(os, windows, linux...)
虛擬機的  優點●節省成本●靈活度與速度●降低停機時間●可擴縮性●安全性優 點
1.VM Ware Workstation：https://www.vmware.com/tw/products/fusion.html2.點選立即  下載安裝虛擬機  （for Windows)
## 安裝虛擬機  （For Mac & M1)1.VM Ware fusion(mac)：https://www.vmware.com/tw/products/fusion.html2.點選免費  試用
