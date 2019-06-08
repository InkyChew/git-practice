# Practice Git

# Local
- 新增、初始 WorkingDirectory
$ cd /code                 # 切換至 /code 目錄
$ mkdir git-practice       # 建立 git-practice 目錄
$ cd git-practice          # 切換至 git-practice 目錄
$ git init         # 初始化這個目錄，讓 Git 對這個目錄開始進行版控

$ git status

- 將檔案放置Staging Area
$ git add –all/.
檔案從 Untracked 變成 new file 狀態

- 將 Staging Area 的內容永久提交到 LocalRepo 裡存檔
$ git commit -m "init commit" # 說明「在這次的 Commit 做了什麼事」
$ git commit -a -m "update content" # 只對已經存在 Repository 的檔案有效

- 檢視 Commit 紀錄
$ git log
$ git log --oneline --author="Sherly|Eddie"
$ git log --oneline --grep="wtf"
$ git log -S "Ruby"
$ git log --oneline --since="9am" --until="12am" --after="2017-01"

# Remote
- 設定遠端節點
$ git remote add origin https://github.com/InkyChew/git-practice.git
- Push
$ git push -u origin master
-u upstream  # 將 origin/master 預設為本地 master 分支的 upstream
