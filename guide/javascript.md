# JavaScript 代码规范

## 命名规则

### 文件命名

- 字母全部小写
- 不要带空格
- 用破折号`-`连接单词
- 库文件可用逗点`.`，用于体现版本或从属关系

#### 示例

- react-router.js
- jquery.min.js
- jquery.form.js
- jquery-1.4.2.js

### 变量名

变量名推荐使用小驼峰法[^CAMELCASE]来命名

#### 示例

```js
const firstName = 'John';
const lastName = 'Doe';

const price = 19.90;
const tax = 0.20;

const fullPrice = price + (price * tax);
```

[^CAMELCASE]: 第一个单词首字母小写，后面其他单词首字母大写。

### 全局变量及常量

全局变量及常量使用全大写的形式命名

#### 示例

```js
const ENV = 'dev'; // 环境为开发环境
```

---

## 空格与运算符

通常运算符 ( = + - * / ) 前后需要添加空格

### 示例

```js
const x = y + z;
const values = ['Volvo', 'Saab', 'Fiat'];
```

---

## 代码缩进

通常使用**2**个空格符号[^SPACE]来缩进代码块

### 示例

```js
function toCelsius(fahrenheit) {
  return (5 / 9) * (fahrenheit - 32);
}
```

[^SPACE]: 不推荐使用**TAB**键来缩进，因为不同编辑器**TAB**键的解析不一样。
