# vue-router-for-everyone

## “dynamic” 是 “动态的意思”

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

#### 1.查看所有(包括本地和远程)分支列表 
```
git branch -a
```
#### 2.只查看远程分支列表
```
git branch -r
```
#### 3.只查看本地分支列表
```
git branch
```

#### 4.删除远程分支
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
## Git创建远程分支
假设当前分支为master，需要创建的分支是my-test

1. git checkout -b my-test  //在当前分支下创建my-test的本地分支分支
2. git push origin my-test  //将my-test分支推送到远程
3. git branch --set-upstream-to=origin/my-test //将本地分支my-test关联到远程分支my-test上   
4. git branch -a //查看远程分支 

此时远程分支my-test已经创建好了，并且本地的分支已经关联到远程分支上
本地push代码以后会push到关联的远程分支上。