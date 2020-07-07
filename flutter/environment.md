# Flutter 开发环境搭建

## 获取Flutter SDK

1. 下载[Flutter SDK](https://flutter.dev/docs/get-started/install)。
2. 解压安装包至安装目录，如：

  ```bash
  cd ~/Library
  unzip ~/Downloads/flutter_macos_1.17.5-stable.zip
  mv flutter Flutter
  ```

3. 进入`～/.zshrc`文件，添加如下代码，将`flutter`相关工具到`path`中。

  ```shell
  # Flutter SDK
  export PATH=$HOME/Library/Flutter/bin:$PATH
  ```

4. 命令行执行`flutter doctor`，检查Flutter SDK是否安装成功（Dart SDK已经在捆绑在Flutter里了，没有必要单独安装Dart）。

## Android Studio 配置

### 安装Flutter和Dart插件

1. 启动Android Studio.
2. 打开插件首选项。
3. 选择*Browse repositories…*, 选择*Flutter*插件并点击*install*.
4. 重启Android Studio后插件生效。

## Visual Studio Code 配置

安装[Flutter](https://marketplace.visualstudio.com/items?itemName=Dart-Code.flutter)插件。
