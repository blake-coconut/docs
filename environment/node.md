# Node.js 环境安装

## 使用 NVM 管理 Node.js 版本

### 安装 NVM

在终端中输入命令：

```bash
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash
```

执行完后在终端中输入`nvm -v`，如果没有正确输出版本号，则需新增配置：

在`.zshrc`文件中添加配置（`.zshrc`文件在自己的用户目录下，没有就新建一个）：

```yml
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
```

### 安装 Node.js

在终端输入命令`nvm install Node.js 版本号`（查看[最新版本](https://nodejs.org/zh-cn/)）。

```bash
nvm install 12.16.2
```

---

## 使用 Yarn 作为 Node.js 的包管理工具

在命令行中输入命令`brew -v`，如果没有正确输出版本号，则需要安装`Homebrew`。

### 安装 Homebrew

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

### 安装 Yarn

```bash
brew install yarn
```
