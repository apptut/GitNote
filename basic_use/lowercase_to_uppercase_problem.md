## 大小写问题

如果`git`版本中把一个`A.txt`文件改为`a.txt`，`git`是不会记录这次更改的，因为`git`不区分同名文件的大小写，很郁闷，只有强制重命名该文件:

```git
git mv --force A.txt a.txt
```
