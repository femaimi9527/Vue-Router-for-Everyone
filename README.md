# vue-router-for-everyone

## “route” 是 “路径，路由的意思”，“router” 是 “路由器的意思” 

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

## Github启用SSH连接：
1. ```git config user.name “你的用户名”```;
2. ```git config user.email “你的注册在github的电子邮箱地址”```;
3. ```ssh-keygen -t rsa -C "femaimi9527@gmail.com"```;
4. ```ssh -T git@github.com```,提示“Hi femaimi9527! You've successfully authenticated, but GitHub does not provide shell access.”则成功;
5. 登录github网站，在setting里面的“SSH and GPG keys”里面，“New SSH key”,把自己电脑的“id_rsa.pub”文件打开，复制以“ssh-rsa...”开头的公钥，粘贴到github，完成;

## Git 的tag的使用：
1. ```git tag v1.0.1 ```,在当前分支下创建一个tag；
2. ```git push origin v1.0.1  ```,把当前分支下创建的tag-v1.0.1推送到github；
3. ```//带信息的tag：-m后面带的就是注释信息，这样在日后查看的时候会很有用
git tag -a v1.0 -m 'first version'```;
4. ```//创建轻量级tag：这样创建的tag没有附带其他信息
git tag v1.0```;
5. ```//我们在执行 git push 的时候，tag是不会上传到服务器的，比如现在的github，创建 tag 后 git push ，在github网页上是看不到tag 的，为了共享这些tag，你必须这样：
git push origin v1.0
或者
//将所有tag 一次全部push到github上。
git push origin --tags```;
6. ```//删除本地tag
git tag -d v1.0```;
7. ```创建一个基于指定tag的分支

git checkout -b tset v0.1.0```;
