# university-learning-plan
## 目录区
- [Git](#git)
- [Blog](#blog)
---
## 内容区
### Git
#### 网课资源:（尚未完成网页跳转）???
b站黑马Git全套教程
#### 基本流程  
<img width="570" height="226" alt="屏幕截图 2026-09-04 225052" src="https://github.com/user-attachments/assets/f212e45b-7df8-4789-bc92-2ec085bf4710" />

#### 基本配置
```bash
git config --global user.name"xxx"
git config --global user.email"xxxxx"
1、touch ~/.bashrc
2、notepad ~/.bashrc或vi ~/.bashrc
3、alias git-log='git log --pretty=oneline --all --graph --abbrev-commit'
4、alias ll='ls -al'
5、source ~/.bashrc
（1~5是取别名）
```
#### 常用指令
```bash
git init;
ll/ls -a;？？？（看目录）
touch file01.txt。或touch .gitignore再vi输入*.a来不允许git管理;
git status;
git add .;
git commit -m "xxx"<-版本名？;
git log，可加--oneline;
git reset --hard commitID(版本号数字)或commit HEAD~1、2...；？（右键复制，ctrl+c是暂停）
git reflog;
vi file01.txt要用i输入，用:wq保持并退出，用:q!退出;
clear
```
#### 分支常用指令
```bash
git branch也可用git log --oneline;
git branch xxx;（补上-a是显示all本地和远程仓库，-r是remote远程仓库，-v是再显示版本号和描述verbose）
git checkout xx(切换分支)。git checkout -b xx(创建并切换)；
git merge xxx(在main上改则是合并xxx至main)（有普通模式和快进模式）
git branch -d xxx;(删除所在分支以外的其他分支，若所删分支未完成merge,可把-d换成-D)
（两条线merge冲突时打开最终文件手动改）
git branch -m master main(master改名为main)
```
#### 分支运用
？？？
<img width="792" height="507" alt="屏幕截图 2026-09-05 114716" src="https://github.com/user-attachments/assets/1ab65141-299b-4c5e-b8d5-64a54f0ac078" />
```bash


```
#### 上传github
```bash
1.在 GitHub 网页上创建一个空仓库
2.打开 VS 的“终端”或系统命令行（PowerShell），用 cd 命令进入你的项目文件夹。？？？
3.（？？？可以先创gitignore排除.vs、x86等等）
  git init
  git add .
  git commit -m "Initial commit"
4.从 GitHub 仓库页面复制仓库地址（HTTPS 或 SSH 格式）
5.git remote add origin <仓库地址>
  git push -u origin main:main（本地main推到云端main，若名字相同可直接写一个main）
？？？（补充）
Visual Studio 项目里的 .vs 文件夹、x64 文件夹等包含本地配置和编译产物，不应该上传到 GitHub，
可以在项目根目录下创建一个 .gitignore 文件，把它们排除掉，这样仓库会更干净
```
### Blog
























