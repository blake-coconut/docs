# 字体图标

## 安装支持中间件

```bash
yarn add react-native-svg
```

安装成功后

```bash
cd ios
pod install
```

## 安装字体转换工具

```bash
yarn add react-native-iconfont-cli --dev
```

安装成功后执行

```bash
npx iconfont-init
```

会在项目根目录生成一个配置文件`iconfont.json`，配置如下

```json
{
  "symbol_url": "请参考README.md，复制官网提供的JS链接",
  "use_typescript": false,
  "save_dir": "./src/iconfont",
  "trim_icon_prefix": "icon",
  "default_icon_size": 18
}
```

执行命令生成图标组件

```bash
npx iconfont-rn
```
