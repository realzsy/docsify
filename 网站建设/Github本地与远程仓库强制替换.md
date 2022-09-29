# Github本地与远程仓库强制替换

> [!note]为了顺利更新远程仓库，和保持本地仓库与远程仓库一致，找了本地与远程互相强制替换的命令。

## 远程仓库强制覆盖本地仓库

```bash
git fetch --all &&  git reset --hard origin/master && git pull
```

- 第一步git fetch --all：拉取所有更新，不同步；
- 第二步git reset --hard origin/master：本地代码同步线上最新版本(会覆盖本地所有与远程仓库上同名的文件)；
- 第三步：再更新一次（非必须）

## 本地仓库强制覆盖远程仓库

```bash
git push origin master --force
```

> [!warning]好像这样操作不是很规范、很安全？我只是为了博客能正常更新，先不管那么多了。



