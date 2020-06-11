# This is ARAM TEAM Blog

> 这里是aram团队的创新实训博客

## docsify博客的使用方法
> 按照以下步骤你将能在自己电脑上本地预览你所写的博客内容

首先你要确保已安装`nodejs`与`git`，下面我们将使用`npm`全局安装`docsify-cli`
请使用终端执行下面的shell命令 

### 下载到本地仓库
首先找到一个合适路径存储git仓库，我们将其克隆到本地，执行
```bash
$ git clone https://github.com/ARAMTEAM/PTMS.git
```
PTMS文件夹保存到了本地，我们
```bash
$ cd PTMS
```
继续进行下面的操作

### 维护自己的博客日志

自己的博客日志再`PTMS`文件夹中的`/aram/your_last_name.md `中，我们记录自己的日志不需要太多的言语，总结好自己的上次更新至本次更新的工作量即可，将新日志更新再markdown的开头部分，详细的工作可以记录到个人CSDN博客上

>注意，这里推荐大家将自己的日志markdown文件复制出来，即你的专属的`your_last_name.md`。每一次填写都在复制出来的`your_last_name.md`文件中编写markdown文件，需要将自己的markdown文件更新时，我们将进行以下操作

### Github pages的更新
首先进入`PTMS`文件夹,依次执行以下命令

>首先更新本地的git仓库，因为git可能在他人提交之后会发生变化
```bash
$ git pull
```
>更新完成后，将自己的`your_last_name.md`文件复制到`/docs/aram/`下覆盖以前的你的日志文件。覆盖完成以后开始进行本地仓库上传到github操作
```bash
$ git add .  #git更新状态树，但不会记录删除的文件
$ git commit -m "引号内填写你本次更新的评论，一般写写自己的近期学习总结梗概即可"
$ git push   #本地仓库push到git仓库
```
只要自己push出错了，一般就是忘记预先pull了，因为别的成员可能在你更新自己的博客日志的时候已经push上他们的文件了，这样你的本地就和git仓库对不起来就会报错。
一般push完以后等待一会儿博客才会更新

### 本地预览博客效果
>如果你想在本地未上传之前就先浏览上传之后的博客效果，或者边浏览最终博客效果便书写markdown的话你就需要在本地安装一下docsify
```bash
$ npm i docsify-cli -g
```
然后将你的`PTMS`仓库文件复制一份出来，例如起个别名`PTMS1`，然后进入`PTMS1`中执行

```bash
$ docsify serve docs
```
就会发现`Listening at http://localhost:xxxx`的输出了，接下来就可以修改你的专属markdown并在`http://localhost:xxxx`下实时预览你的最终博客效果了

### 想要添加文档补充项目信息
>1. 首先在`/docs/posts/`文件夹中新建相关的markdown文件（这里和更新一样还是推荐其他文件夹下写完pull以后加到本地仓库后再push）
2. 在`/docs/`下的`_sidebar.md`中添加一行
    ```
    * [你想展示文件内容的标题](posts/你的markdown文件.md)
    ```
然后左侧侧边栏就会更新你的内容了

### 结尾
以上就是博客更新的内容了，想要了解docsify详细操作请前往https://docsify.js.org/ 官网学习。
自己辛苦写完的日志一定要记得push上去并更新呀😀