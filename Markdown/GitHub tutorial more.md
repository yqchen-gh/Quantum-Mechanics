# GitHub进阶

以下部分出自笑来老师的新书[自学是门手艺](https://github.com/selfteaching/the-craft-of-selfteaching/)，如果能帮到自己的话，就去原作者那里给个Star吧～

需要说明的是，文档中对应的主仓库是`selfteaching/the-craft-of-selfteaching`，而我们这里的主仓库是`YQChen-QI/Quantum-Mechanics`，阅读的时候自行替换一下就行了。

## 如何使用 Pull Request 为本仓库做贡献

(1) 使用浏览器访问 [the-craft-of-selfteaching](https://github.com/selfteaching/the-craft-of-selfteaching)

(2) 点击右上角的 “Fork 按钮”，将该仓库 Fork 到你的 Github 账户中

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/github-fork.png?raw=true)

(3) 创建一个新分支，可以取名为 `from-<your_username>`，比如，`by git.basic.tutorial`；之后点击 Create Branch 建立新分支。

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/github-new-branch.png?raw=true)

(4) 在新分支下进行修改某个文件，而后提交 —— 提交前不要嫌麻烦，一定要在 Comment 中写清楚修改说明：

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/github-commit.png?raw=true)

以上示例图片中是修改了 README.md 文件 —— 事实上，你应该提交的是的确有必要的校对。

另外，**请注意**：在创建分支之前，要将你的 Fork 更新到最新版。具体操作方法见下一节《如何在 Github 网站上将自己的 Fork 与原仓库同步》。

(5) 在页面顶部选择 Pull request 标签：

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/github-pull-request.png?raw=true)

而后点击 `Compare & pull request` 按钮 —— 如果看不到这个按钮，那就点击下面刚刚修改文件的链接，如上图中的 “Update README.md”（这是你刚刚提交修改时所填写的标题）。

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/github-open-pull-request.png?raw=true)

确认无误之后，点击 `Create pull request` 按钮。

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/github-create-pull-request.png?raw=true)

(6) 随后，Github 用户 [@xiaolai](https://github.com/xiaolai) —— 就是我，即，the-craft-of-selfteaching 这个仓库的所有者，会被通知有人提交了 Pull request，我会看到：

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/github-confirm-merge.png?raw=true)

在我确认这个 Pull request 修改是正确的、可接受的之后，我就会按 `Merge pull request` 按钮 —— 如此这般，一个修正就由你我共同完成了。

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/github-merged-pull-request.png?raw=true)

**注意**

提交 Pull request 的时候，最佳策略如下：

> * 提交 Pull request 之前，必须先将你的 Fork 的 master 与原仓库同步到最新；
> * 从 master 创建 **新的 branch** 进行增补、修改等操作；
> * 尽量每次只提交一个小修改；
> * 提交时尽量简短且清楚地说明修改原因；
> * 耐心等待回复。

当自己的 Fork 过来的仓库已经被你在本地 “玩残” 了的时候，它千万不能被当作用来提交 Pull request 的版本。自己本地怎么玩都无所谓，但需要向别人提交 Pull request 的时候，必须重新弄一个当前最新版本到本地，而后再在其基础上修改。

## 如何在 Github 网站上将自己的 Fork 与原仓库同步

(1) 在你的 Fork 页面中如下图所示，点击 `Compare` 链接：

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/sync-fork-1.png?raw=true)

(2) 将 `base repository` 更改成当前自己的 Fork，在图示中即为 `gitbasictutorial/the-craft-of-selfteaching`：

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/sync-fork-2.png?raw=true)

(3) 这时候，页面会显示 `There isn't anything to compare.`，因为你在比较 “自己” 和 “自己”。点击 `compare across forks` 链接：

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/sync-fork-3.png?raw=true)

(4) 将 `head repository` 更改成 Upstream Repository（即，上游仓库），在图示中即为 `selfteaching/the-craft-of-selfteaching`：

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/sync-fork-4.png?raw=true)

(5) 稍等片刻，你会看到比较结果；而后你可以创建一个 Pull request —— 这是一个由你自己向你自己的 Fork 仓库提交的 Pull request：

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/sync-fork-5.png?raw=true)

(6) 而后你在 `Pull requests` 标签页里会看到你刚刚提交的 Pull request：

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/sync-fork-6.png?raw=true)

(7) 同意并合并之后的结果是，你的 Fork 与上游仓库同步完成了：

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/sync-fork-7.png?raw=true)

当然，有时会出现一些你无法解决的问题，那么，还有一个最后的方法：

> 将你的 Fork 删除，而后重新到 https://github.com/selfteaching/the-craft-of-selfteaching 页面按一次 `Fork` 按钮……

## 如何使用 github 记录自己的学习过程

你可以在本地建立一个分支（branch），例如，取名为 `study`：

```bash
git branch study
git checkout study
```

如此这般之后，你在本地工作目录中所做的任何修改，都可以提交到 `study` 这个分支之中。

你每次在 Jupyterlab 中浏览 `ipynb` 文件，按 `^ + Enter` 执行 code cell 中的代码的时候，该文件都会发生一些变化；你也可以随意修改文件中的任何地方，比如，添加一个 code cell，将某段代码从头至尾 “敲” 一遍；也可以修改某个 code cell 中的代码看看执行结果有什么不同；还可以添加或者修改任何 markdown cell —— 就当自己做笔记了……

总而言之，当你阅读完某一章节并如上所说那样做了一些改动之后，那个 `ipynb` 文件就发生了一些变化。于是，你就可以执行以下命令：

```bash
git add .
git commit -am 'my study result'
git push
```

如此这般，在 `study` 这个分支中就记录着你的学习轨迹。

当然，如果在这过程中，你发现本书自身有需要校对的地方，那么，你需要切换到 `master` 分支，执行以下命令：

```bash
git checkout master
git pull
```

而后再修改，进而按照上一节的方法提交 Pull request。

未来，在 [https://github.com/selfteaching](https://github.com/selfteaching) 下我会专门设置一个 repo，用来自动扫描 github 上本书的学习记录 —— 这种记录在过往的书籍当中是不可能存在的，然而，现在却可以了。在我看来，将来这种记录的作用甚至有可能比 “学历” 还要重要。
