# prettier-rules

常用的 [`prettier`](https://prettier.io/docs/en/configuration.html) 规则


## 使用方式

### 安装依赖
```
npm i @hkt/prettier-rules prettier -D
```

### 配置 prettier

根目录下创建 `.prettierrc.js`

```
module.exports = require('@hkt/prettier-rules');
```

## 搭配 eslint 使用
通常我们的项目都是有 `eslint` 的，`prettier` 可以搭配它一起使用

### 安装依赖

```
npm i @hkt/prettier-rules eslint-config-prettier eslint-plugin-prettier -D
```

#### 在 eslint 中配置 `prettier`
找到 `eslint` 配置文件，如：`.eslintrc.js`。在 `extends` 中加入 `prettier`

```
module.exports = {
  extends: ['./node_modules/@hkt/eslint-rules/react.js', './node_modules/@hkt/eslint-rules/jsx-a11y.js', 'prettier'],
};

```
