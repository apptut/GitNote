## 常用命令

#### 1.rebase

合并多个commit为一个commit提交：

```
$ git log --pretty=oneline
897fa79def2cf256b7f14d0ec0fcb67e8f61a814 test_rebase5
7dff3e4ad7416f0370b4579393a0c8a8fc02efbd test_rebase4
37be873b514afd9d8f6536cd893eadc3e32b4966 test_rebase3
5ae88f5a0454066d820f6c1687b6d01f59f39dbd test_rebase2
128a2f5cdb325bcbdb26b35741fad2a2fba49832 test_rebase1
```
把以上5个commit合并为一个commit提交：

```
git rebase -i HEAD~5
```

#### 2.设置自动纠错

设置为1的时候，如果只有1个命令被模糊匹配到，将自动纠错。

```
git config --global help.autocorrect 1
```

#### 3.设置高亮

```
git config --global color.ui auto
```

#### 4.设置命令别名

如果一条命令很长或者很难记，那么我们可以为他设置一个别名。

```
git config --global alias.st status
```
