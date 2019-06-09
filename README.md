# Notes

<h3>Git 基本觀念</h3>

![Git基本觀念](https://blog.techbridge.cc/img/kdchang/cs101/git-workflow.png)

<h3>新增、初始 WorkingDirectory</h3>
    
    $ cd /code            # 切換至 /code 目錄
    $ mkdir git-practice  # 建立 git-practice 目錄
    $ cd git-practice     # 切換至 git-practice
    $ git init            # 初始化目錄，讓 Git 開始對目錄進行版控
    


`$ git status  # 查詢目錄狀態`

<h3>將檔案放置 Staging Area</h3>

`$ git add –all/.  # 檔案從 Untracked 變成 new file 狀態`

<h3>將 Staging Area 的內容永久提交到 LocalRepo 裡存檔</h3>
    
    $ git commit -m "init commit"        # 說明此次 Commit 做了什麼事
    $ git commit -a -m "update content"  # 只對已經存在 Repository 的檔案有效
    
<h3>檢視 Commit 紀錄</h3>
    
    $ git log
    $ git log --oneline --author="Sherly|Eddie"
    $ git log --oneline --grep="wtf"
    $ git log -S "Ruby"
    $ git log --oneline --since="9am" --until="12am" --after="2017-01"
    
<h3>Push</h3>
    
    $ git remote add origin https://github.com/InkyChew/git-practice.git  # 設定遠端節點
    $ git push -u origin master
    # -u upstream 將 origin/master 預設為本地 master 分支的 upstream

<h3>Pull</h3>

> _git pull = git fetch + git merge_

# Reference
- https://gitbook.tw/
- https://blog.techbridge.cc/2018/01/17/learning-programming-and-coding-with-python-git-and-github-tutorial/
