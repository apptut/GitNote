## tab 自动提示

bash默认是没有实现`git`命令的自动完成，因此需要自己来实现一个：

1. 下载一个自动脚本

```sh
curl -k https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash -o ~/.git-completion.bash
```
2. 在`.bash_profile`添加如下代码，并且执行`source .bash_profile`：

```sh
if [ -f ~/.git-completion.bash ]; then
  . ~/.git-completion.bash
fi
```


