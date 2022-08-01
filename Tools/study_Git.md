# gitskills
Git学习笔记

## 安装Git
Mac 上如果安装了最新的XCode，可以使用XCode进行安装。

Ubuntu中可以使用<code>sudo apt-get install git</code>命令来进行安装。

## 创建版本库

<pre>
  mkdir selfgit
  cd selfgit
  git init
</pre>

把文件添加到版本库中可以使用 `git add filename`
然后使用 `git commit -m "comments"` 提交到版本库中

使用 `git status` 命令可以查看版本库当前的状态。

使用 `git diff filename` 命令可以查看具体修改什么内容。

## 克隆远程库

如克隆github上的远程库gitskills

`git clone git@github.com:yourname/gitskills.git`

## 分支

对于一个任务需要较长时间完成，如果等全部完成后再提交到库中可能会面临这个任务过程中工作的丢失，这个时候可以使用分支建立对这个任务的版本管理，等到任务全部完成后，一次性合并到原来的库（分支）上，这样既安全又不影响别人的工作。

Git 鼓励大量使用分支：

查看分支： <code>git branch</code>

创建分支： <code>git branch &lt;name&gt;</code>

切换分支： <code>git checkout &lt;name&gt;</code>

创建＋切换分支： <code>git checkout -b &lt;name&gt;</code>

合并某分支到当前分支： <code>git merge &lt;name&gt;</code>

删除分支： <code>git branch -d &lt;name&gt;</code>

当合并分支的时候产生冲突，需要首先解决冲突，然后再进行合并。

用`git log --graph`命令可以看到分支合并图。


