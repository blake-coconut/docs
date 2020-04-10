# Prettier

代码格式化程序。

## 使用方式

1. 在`Visual Studio Code`中安装插件[Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)。
2. 在`Visual Studio Code`系统设置中，将选择`editor.formatOnSave`改为`true`；同时选项`files.autoSave`的值不能为`autoSaveDelay`。
3. 在项目中使用命令`yarn add prettier --dev`或`npm install prettier --save-dev`安装依赖。
4. 在项目根目录添加`prettier`的配置文件`.prettierrc`，带有可选扩展名：（`.json/.yaml/.yml/.js`无扩展名优先）。
5. 在配置文件中添加如下配置。（为了示例中的注释，使用的`js`代码，实际运用请改为`json`格式）。

推荐的配置项：

```js
module.exports = {
  printWidth: 80, // 一行代码的长度
  tabWidth: 2, // 缩进的空格数
  useTabs: false, // 使用制表符而不是空格进行缩进
  semi: true, // 在语句末尾加上分号
  singleQuote: true, // 使用单引号而不是双引号
  quoteProps: 'as-needed', // 对对象中key的引号规范
  jsxSingleQuote: false, // 在JSX中使用单引号而不是双引号
  trailingComma: 'es5', // 多行时尽可能打印尾随逗号（例如：单行数组永远不会出现逗号结尾）
  bracketSpacing: true, // 在对象文字中的括号之间打印空格（例如：{ age: 18 }）
  jsxBracketSameLine: false, // JSX Brackets。文档有例子，转去文档看直观一些
  arrowParens: 'always', // 在单独的箭头函数参数周围包括括号
  endOfLine: 'lf', // 行结束
};
```

更多配置请查阅[文档](https://prettier.io/docs/en/options.html)。
