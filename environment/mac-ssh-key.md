# Mac 系统下查看和生成 SSH Key

1. 打开终端，先查看是否存在`SSH Key`。

```bash
ls -al ~/.ssh
```

如果输出的是如下内容：证明本地没有生成的`SSH Key`，请执行第二步。

```bash
No such file or directory
```

如果输出的是如下内容：证明本地已经存在`SSH Key`文件，请执行第四步。

```bash
id_rsa        id_rsa.pub
```

2. 如果没有，生成新的`SSH Key`。

```bash
ssh-keygen -t rsa -C"you_email"
```

`your_email`：这里填写你在GitLab或者GitHub注册时的邮箱，后面的提示直接敲回车，一路完成。

3. 生成并添加`SSH Key`。

```bash
ssh-add ~/.ssh/id_rsa
```

4. 查看`SSH Key`。

```bash
cat /Users/xxx/.ssh/id_rsa.pub
```

`xxx`是你的电脑用户名。
