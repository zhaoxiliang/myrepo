# 这是关于 git使用的练习(new)


### 设置Git, Github

1. 创建仓库

登入Github.com，新建仓库：myrepo， 选择public, Initialize this respository with README， 然后点南击绿色的“创建仓库”。

2. 克隆到自己的计算机
 打开shell，可以在RStudo中，Tools > Shell方式打开。
看看当前目录位置 pwd，可以通过cd进入自己想要的目录，我是进入的
/Users/zhaoxiliang/Github（苹果电脑）

将github仓库myrepo克隆到本地

git clone https://github.com/zhaoxiliang/myrepo.git

将该目录作为新的工作目录
 - cd myrepo
 - ls
 - less README.md # press [q] to quit
 - git remote show origin

3. 在本地修改文件，commit， and push
加一行内容

 - echo “A line I wrote on my local computer” >> README.md
 - git status

Commit this change and push to your remote repo on GitHub

 - git add -A
 - git commit -m “A commit from my local computer”
 - git push

第一次推送要输入github的用户名和密码。

4. 到Github仓库浏览变动，可能需要刷新页面。应该可以看到README.md多了一行信息。


5. 删除本地仓库
 - cd ..
 - rm -rf myrepo/

在Github页面删除仓库。由Settings， 向下翻，在最底部点击“Delete this repository”。
