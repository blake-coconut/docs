# React Native 开发环境搭建

## 准备 Node.js 环境

参考文档[Node.js 环境安装](environment/node)

---

## 安装依赖

使用[Homebrew](https://brew.sh/)安装`Watchman`，在终端运行命令：

```bash
brew install watchman
```

[Watchman](https://facebook.github.io/watchman/)是Facebook的一种工具，用于监视文件系统中的更改。

---

## 安装 Xcode

通过[Mac App Store](https://apps.apple.com/us/app/xcode/id497799835?mt=12)安装`Xcode`。

### 安装命令行工具

打开`Xcode`，在菜单中选择`Preferences...`，转到`Locations`面板，通过在`Command Line Tools`，下来列表中选择最新版本来安装工具。

### 安装 iOS 模拟器

打开`Xcode`，在菜单中选择`Preferences...`，转到`Components`面板，选择一个相应的`iOS`版本的模拟器。

### 安装 CocoaPods

[CocoaPods](https://cocoapods.org/)是使用Ruby构建的，可以使用macOS上可用的默认Ruby安装。在终端运行命令：

```bash
sudo gem install cocoapods
```

---

## Java JDK

使用[Homebrew](https://brew.sh/)安装JDK。在终端运行命令：

```bash
brew cask install adoptopenjdk/openjdk/adoptopenjdk8
```

---

## 安装 Android Studio

下载并安装[Android Studio](https://developer.android.com/studio/index.html)，提示选择安装类型时，选择“自定义”设置。选中以下所有选项：

- `Android SDK`
- `Android SDK Platform`
- `Performance (Intel ® HAXM)`
- `Android Virtual Device`

然后，单击“下一步”以安装所有这些组件。

---

## 初始化 React Native 项目

使用以下命令，初始化一个`TypeScript`模板的 React Native 项目：

```bash
npx react-native init ProjectName --template react-native-template-typescript
```

---

参考[React Native 官方文档](https://reactnative.dev/docs/environment-setup)
