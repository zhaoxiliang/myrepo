# 这是关于 git使用的练习

![](https://d33wubrfki0l68.cloudfront.net/b88ef926a004b0fce72b2526b0b5c4413666a4cb/24a30/cover.png)


书本链接地址：[R for Data Science](https://r4ds.had.co.nz)

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

6. Git pull
可以在Github上fork别的仓库，然后clone到本地，修改后，git push到自己的fork的仓库，最后pull请示，进行合并请示和更新？
A line I wrote on my local computer
