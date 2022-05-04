# yarn-codes

## yarn set version berry 失败

> Error: getaddrinfo ENOENT raw.githubusercontent.com raw.githubusercontent.com:443

1. 查找 ip，需要查出 raw.githubusercontent.com 的真实 IP，进入这个网址：https://www.ipaddress.com/
2. 修改 hosts 文件，打开文件：C:/Windows/System32/drivers/etc/hosts

3. 在最后添加 199.232.68.133 raw.githubusercontent.com
4. 注意用自己的查到的 ip，修改 hosts 注意权限问题
5. 再次运行 yarn set version berry，成功安装。

## 用法

### 显示命令列表

```
yarn help

```

### 初始化一个新项目

```
yarn init

```

### 安装所有依赖项

```
yarn
yarn install

```

### 添加依赖项

```
yarn add [package]
yarn add [package]@[version]
yarn add [package]@[tag]
```

### 将依赖项添加到不同的依赖类别中

```
yarn add [package] --dev  # dev dependencies
yarn add [package] --peer # peer dependencies
```

### 更新依赖项

```
yarn up [package]
yarn up [package]@[version]
yarn up [package]@[tag]
```

### 删除依赖项

```
yarn remove [package]
```

### 更新 Yarn 本体

```
yarn set version latest
yarn set version from sources
```
