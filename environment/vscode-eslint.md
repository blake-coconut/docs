# 在 VSCode 中配置 ESLint

1. 在`VSCode`中下载扩展[ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)。
2. 在`VSCode`设置中添加如下设置：

  ```json
  {
    "editor.formatOnSave": true,
    "editor.codeActionsOnSave": {
      "source.fixAll.eslint": true
    },
    "eslint.enable": true,
    "eslint.debug": true,
    "eslint.packageManager": "yarn",
    "eslint.run": "onType",
    "eslint.alwaysShowStatus": true
  }
  ```

3. 进入项目根目录，使用`yarn`命令安装以下依赖：`yarn add eslint eslint-config-airbnb eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react eslint-plugin-react-hooks --dev`
4. 在项目跟目录新建配置文件`.eslintrc.js`，并复制以下配置至配置文件（以下配置会按需进行更新）：

  ```js
   module.exports = {
    root: true,
    extends: [
      'airbnb',
    ],
    globals: {
      cc: true,
    },
    rules: {
      'max-len': [1, 80],
      'no-underscore-dangle': [2, { allowAfterThis: true }],
      'no-multiple-empty-lines': [2, { max: 1 }],
    }
  };
  ```
