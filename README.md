# Git Tutorial

- [Git Tutorial](#git-tutorial)
  - [01 Local Repository](#01-local-repository)
  - [02 Remote Repository](#02-remote-repository)

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

Reference:

- https://ithelp.ithome.com.tw/users/20139195/ironman/4770
