# iTerm2 与 Oh My Zsh 配置

## 下载 iTerm2

在[iTerm2 官网](https://www.iterm2.com/)下载安装`iTerm2`，使用以下命令，将系统默认终端修改为`zsh`：

```bash
chsh -s /bin/zsh
```

---

## 安装 Oh My Zsh

使用下面两种方式安装：

```bash
# curl 安装方式
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

或

```bash
# wget 安装方式
sh -c "$(wget https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"
```

[Oh My Zsh 官方地址](https://github.com/ohmyzsh/ohmyzsh)

---

## 设置主题

进入`~/zshrc`文件，将`ZSH_THEME=""`修改为`ZSH_THEME="ys"`，或自己喜欢的主题，可查看[Oh My Zsh 主题列表](https://github.com/ohmyzsh/ohmyzsh/wiki/Themes)。

---

## 设置字体

1. 为了避免乱码，需要`Meslo`字体支持，[下载字体](https://links.jianshu.com/go?to=https%3A%2F%2Fgithub.com%2Fpowerline%2Ffonts%2Fblob%2Fmaster%2FMeslo%2520Slashed%2FMeslo%2520LG%2520M%2520Regular%2520for%2520Powerline.ttf)。
2. 下载完毕后直接点击安装。
3. 打开`iTerm2`偏好设置，然后选择`Profiles -> Text -> Font -> Chanage Font`，选择`Meslo LG M Regular for Powerline `字体。

---

## 安装插件

命令选择、补全插件：

```bash
cd ~/.oh-my-zsh/custom/plugins/
git clone https://github.com/zsh-users/zsh-autosuggestions
```

语法高亮插件：

```bash
cd ~/.oh-my-zsh/custom/plugins/
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git
```

下载完后打开`~/.zshrc`文件，将插件配置修改为`plugins=(git zsh-autosuggestions zsh-syntax-highlighting)`。

---

## 设置 iTerm2

1. 设置透明度：`Preferences -> Profiles -> Window`拖动`Transparency`。
2. 设置呼出方式：`Preferences -> Profiles -> Style`为`Full-Width Top of Screen`。
3. 设置呼出屏幕：`Preferences -> Profiles -> Screen`为`Main Screen`。
4. 设置呼出快捷键：`Preferences -> Keys -> Hotkey`为`cmd + ↓`。
5. 设置默认终端：`iTerm2 -> Make iTerm2 Default Term`。
