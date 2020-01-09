# vue-router-for-everyone

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your tests
```
npm run test
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


## Git删除本地分支和远程分支
### (1)删除本地分支：

#### 1.查看本地分支列表
```
git branch
```

#### 2.删除本地分支
```
git branch -d 分支名称
```

### (2)删除远程分支：

#### 1.查看远程分支列表
```
git branch -a
```
#### 2.删除远程分支
```
git push origin --delete 远程分支名称
```
## Git拉取远程分支

```
git pull origin
```
## Git推送数据到远程仓库

```
git push [remote-name] [branch-name]
```

## Git在github创建某分支的新分支
1. 去到某分支；
2. 点击“Branch：...”;
3. “find or create a branch...”;
4. 输入新分支名称，Enter回车键，完成。