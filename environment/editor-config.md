# EditorConfig

统一不同编辑器的编码风格

## 使用方式

1. 在`Visual Studio Code`中安装扩展[EditorConfig for VS Code](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig)
2. 在项目根目录添加配置文件`.editorconfig`

## 推荐配置

```yml
# 官方地址：https://EditorConfig.org

root = true # 表示是最顶层的配置文件，发现设为true时，才会停止查找.editorconfig文件

# 配置所有文件
[*]
trim_trailing_whitespace = true # 修剪尾随空白
indent_style = space # 缩进方式为空格
indent_size = 2 # 缩进长度为2个空格
end_of_line = lf # 保证在任何操作系统上都有统一的行尾结束字符
charset = utf-8 # 文件编码方式
insert_final_newline = true # 是否在文件末尾插入一个空行

# js文件
[*.js]
max_line_length = 80 # 一行最大长度
```
