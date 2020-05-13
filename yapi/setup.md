# MongoDB

```shell
# 由于 MongoDB 不开源了，需要先设置下第三方仓库
brew tap mongodb/brew

# 安装社区版本
brew install mongodb-community

# 启动 MongoDB 服务
brew services start mongodb-community

# 进入 MongoDB
mongo

# 创建数据库（yapi 为数据库名）
use yapi

# 查看当然数据库
db

# 创建用户
db.createUser({user:"admin", pwd:"admin", roles:[{role:"readWrite", db:"yapi"}]})
```

## MongoDB 其他常用命令

```shell
# 重启 MongoDB 服务
brew services restart mongodb-community

# 停止 MongoDB 服务
brew services stop mongodb-community
```

---

# 部署 Yapi

```shell
# 安装 yapi-cli 工具
yarn global add yapi-cli

# 创建文件夹
mkdir yapi

# 进入文件夹
cd yapi

# 克隆代码到 vendors 目录
git clone https://github.com/YMFE/yapi.git vendors

# 复制配置文件
cp vendors/config_example.json ./config.json

# 进入 vendors 目录
cd vendors

# 安装依赖
yarn install

# 安装 Yapi
npm run install-server
```

复制完配置文件后，先修改如下配置：

```js
{
  "port": "7000",
  ...
  "db": {
    ...
    "DATABASE": "yapi",
    "user": "admin",
    "pass": "admin",
    ...
  },
  ...
}
```

## 升级 Yapi

```shell
cd {项目目录}

# 查看版本列表
yapi ls

# 更新到最近列表
yapi update
```

---

# PM2

安装`pm2`

```bash
yarn global add pm2
```

修改 yapi 的 package.json

```json
{
  "script": {
    "start": "pm2 start 'server/app.js' --name yapi",
    "info": "pm2 info yapi",
    "stop": "pm2 stop yapi",
    "restart": "pm2 restart yapi"
  }
}
```
