# Git Tutorial

- [Git Tutorial](#git-tutorial)
  - [01 Local Repository](#01-local-repository)
  - [02 Remote Repository](#02-remote-repository)
  - [03 Clone](#03-clone)
  - [04 Pull](#04-pull)
  - [05 Checkout](#05-checkout)
    - [05-1 HEAD](#05-1-head)
    - [05-2 Branch](#05-2-branch)

## 01 Local Repository

步驟(Windows):

1. `cd FolderPath`
2. `git init`: 初始化
3. `git status`: 查看狀態
4. `git add .`: 將資料夾中的檔案加入Index
   1. or `git add FilePath`
5. `git commit -m "MessageContent"`: 從Index commit到local repository
6. 使用`git status`查看狀態
7. `git log`可以查看完整的commit資訊

## 02 Remote Repository

步驟:

1. 登入[GitHub](https://github.com/)
2. Create new repository
3. 依照指令進行push existing repository
   1. `git remote add YourRepositoryURL`
   2. `git branch -M main`
   3. `git push -u origin main`
4. 完成上傳

## 03 Clone

將GitHub上的Remote repository下載到本機。

步驟:

1. 先到repository的`code`標籤中複製URL
   ![clone](./img//p001_clone_url.png)
2. 輸入指令: `git clone https://github.com/dan61013/Python_practice.git`
3. 完成Clone

## 04 Pull

> 通常用於多人協作時，當需要拉取最新版本時使用。

指令: `git pull origin main`

## 05 Checkout

### 05-1 HEAD

> HEAD指的是當前所在的分支(branch)

到目前為止，練習過程中只有新增一個branch，也就是`main`

而在`main`當中也會有多次commit的紀錄，可以透過指令進行版本切換

指令:

1. 可以用`type .git\HEAD`進行查看當前所在的branch
   1. 或是用`git log`可以同時查詢到HEAD指向與版本SHA-1編號
2. 輸入`git checkout CommitSHA-1`就可以切換到指定的版本號
3. 回到最新版本的方式可以省略版本號，即輸入`git checkout main`

### 05-2 Branch

> 透過Branch避免被其他人commit覆蓋的情形發生，

1. 先新增branch `git branch BranchName`
2. 切換到新增的branch(*develop*) -> `git checkout develop`

Reference:

- https://ithelp.ithome.com.tw/users/20139195/ironman/4770
