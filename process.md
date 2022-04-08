本小组一共有三人，分别是：
- 卫依 41911087（组长）
- 李雨 41911089
- 董文佳 41911166

### 步骤：
### 一、组长创建仓库并将相关内容存入仓库
**组长part：**
1.	在本地创建仓库并初始化
```
cd /d/Git/teamwork
git init
```
2.	分析小组项目的“四个象限”并编写markdown程序存入工作目录
3.	把文件提交到本地仓库
```
git add quadrant.md
git commit -m 'My first commit'
```
4.  在GitHub创建名为teamwork的远程仓库
5.  将本地仓库的内容提交到GitHub的远程仓库
```
git remote add origin git@github.com:Crescentss/teamwork.git
git push -u origin master
```

### 二、组员fork组长的仓库，对仓库内容进行修改后再pull request
**组员part：**

***董文佳***
1.	打开组长的github链接点击‘fork’，将远程仓库teamwork复制到自己的github中。
2.  在本地clone远程仓库teamwork。
```
git clone https://github.com/dwj2001/teamwork.git
```
3.  在本地修改文件内容并保存修改。
4.  将修改后的文件传入远程仓库中。
```
git add quadrant.md
git commit -m '对第一象限第三点进行补充'
git push origin master
```
5.  发起Pull Request并通知组长。在fork远程仓库，点击Pull Request->New Pull Request->Create Pull Request，等待组长回应。

***李雨***
1.	打开组长的github链接点击‘fork’，将远程仓库teamwork复制到自己的github中。
1.  在本地clone远程仓库teamwork。
'''
git clone git@github.com:LiYu0105/teamwork.git
'''
3. 在本地打开文件进行修改并保存。
4. 将修改过后的文件传入仓库。
```
git add quadrant.md
git commit -m '第三象限进行修改'
git remote rm origin
git remote add origin git@git.zhlh6.cn:LiYu0105/teamwork.git
git push origin master
```
5. 在github新添加一个文件，尝试组长是否能收到。
6. 在github发起pull request，并在会话框补充说明。然后等待组长的回应。

### 三、组长对修改后的仓库进行合并
**组长part：**
1.  收到组员pull request请求，对组员提交的内容进行审查
2.  审查无误，进行Merge pull request并Confirm merge，完成合并