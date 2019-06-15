# 0.环境准备

* 安装git
  * [git-book](https://git-scm.com/book/zh/v1)
  * [git 协作流程](http://www.ruanyifeng.com/blog/2015/12/git-workflow.html)
* [安装VS code 并安装Leetcode 插件](https://zhuanlan.zhihu.com/p/56226189) 可选，也可以用IDE刷；
* 安装[typora](https://www.typora.io/)。一个markdown编辑器，所有题解均用markdown编写；

# 1.规约

## 1.1 版本规约

* Java。版本使用java 7 / 8；
* Python。统一使用python3；

## 1.2 准入规约

* 在Leetcode题解平台ac掉该题目
* 需要得到**至少一人**的LGTM(look good to me)才能证明你的代码和题解是OK的。

# 2 参与步骤

## 2.1 获取源码

点击左上角的 `fork` 按钮, 复制一份代码到你的账号仓库下。

## 2.2 拉分支

* clone code下载代码到本地，这一步您可以选择git/https方式

```java
git clone git@github.com:Acceml/LeetcodeTraining.git
```

* 添加分支名称。例如195题题解可以命名如下。。

```
git branch ans_195
```

* 执行完上述命令后，您的代码仓库就切换到相应分支了。执行如下命令可以看到您当前分支：

```
git branch -a
```

- 如果您想切换回主干，执行下面命令：

```
git checkout -b master
```

- 如果您想切换回分支，执行下面命令：

```
git checkout -b ${branchName}
```

## 2.3 修改代码提交到本地

拉完分支后，就可以修改代码了。

* 添加题解。题解命名规范统一示例如下。

```
touch 297.二叉树的序列号与反序列号.md
git add 297.二叉树的序列号与反序列号.md
```

* 修改题解。直接在原来的题解上修改即可。

修改完后。采用如下命令格式提交到本地：

```
git commit -am '添加xx题解'
git commit -am '修复xx题解bug'
```

## 2.4 提交代码到远程仓库

```
git push origin ${branchname}
```

如果前面您是通过 fork 来做的，那么**这里的 origin 是 push 到您的代码仓库，而不是Leetcode的的代码主仓库**。

## 2.5 提交合并代码到主干的请求

在的代码提交到 GitHub 后，您就可以发送请求来把您改好的代码合入 LeetcodeTraning 主干代码了。此时您需要进入您的 GitHub 上的对应仓库，按右上角的 `pull request` 按钮。选择目标分支，一般就是 master，系统会通知 LeetcodeTraning 的维护人员， 对您的代码进行review，符合要求后就会合入主干，成为 LeetcodeTraning 的一部分。

## 2.6 代码 Review

@Acceml。学弱

@赵越越。学霸

@风暴之灵。学神

提交merge request 之后可以在群里@ 相应的同学帮你review，如果需要修改，直接用git进行comment。收到**LGTM**回复后你的题解就可以在公众号上被看到了。

# 鸣谢

群里的各种小伙伴，大家一起进步啊~~~~