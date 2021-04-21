**拉取远程仓库到本地**

在本地新建一个文件夹 `./test`，进入文件夹，右键`git bash here`

```
git init // 初始化
```

假设要拉取的仓库地址为https://github.com/rederxz/mreeg.git，分支名为`main`

```bash
git remote add origin https://github.com/rederxz/mreeg.git
git pull origin main
```

就把仓库拉取到`./test`文件夹中了



**将本地代码提交至远程仓库**

git将本地仓库分为工作区和暂存区，工作区就是本地文件夹中我们可以直接看到的那些文件。在提交代码时，首先要将修改的文件提交至暂存区，再由暂存区提交至远程的仓库。

假设本地的仓库文件夹为`./test`，新增了文件`test.txt`，本次提交的说明文字为`This is a test.`

进入文件夹，右键git bash。首先将该文件提交至暂存区

```bash
git add test.txt 
```

创建一次提交，注意：说明文字的内容要用英文引号包住。

```bash
git commit -m 'This is a test.'
```

提交至`origin`的`main`分支

```bash
git push origin main
```



git暂存区与工作区 https://segmentfault.com/a/1190000017794371

利用git多人协作 https://segmentfault.com/a/1190000019714354



![最常用的GitHub操作](https://xzreder.oss-cn-beijing.aliyuncs.com/img/20190303150053205.png)



