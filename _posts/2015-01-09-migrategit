---
layout: post
title: 迁移Git的托管服务器
---

在偶尔的情况下，我们需要迁移托管在某个git服务器上的内容到另外一个git服务器器，但是想保留之前所有的信息，包括分支，comments等。我们可以用下面的命令来做：

1）git clone --bare git@github.rtp.raleigh.ibm.com:pmc-project/bss.git

从源repository拉下来当前的repository，拉下来的repository的目录为XX.git形式，这里是bss.git.

2）cd bss.git/

3). git push --mirror git@gitlabhost.rtp.raleigh.ibm.com:PMC/bss.git

把拉下来的repository推到想要放置的repository上

稍微做一下解释，--bare参数创建的拉下来的版本库不包含工作区，直接就是版本库的内容，这样的版本库称为裸版本库。一般约定俗成裸版本库的目录名以.git做后缀，所以上面示例中将克隆出来的裸版本库目录名为bss.git.


