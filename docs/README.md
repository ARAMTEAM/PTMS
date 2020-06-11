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
$ git add .
```

```bash
$ npm i docsify-cli -g
```
