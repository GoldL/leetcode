##### 1. 搭建es6环境
- 配置`babel`
```
# 下载依赖
npm i @babel/core @babel/preset-env -D
# 创建babel.config.js
module.exports = {
  presets: [
    [
      '@babel/preset-env',
      {
        targets: {
          node: 'current'
        }
      }
    ]
  ]
}
```
- 配置`jest`
```
# 下载依赖
npm i jest babel-jest -D 
```
- 配置`eslint`
```
# 下载依赖
npm i eslint eslint-config-standard eslint-plugin-import eslint-plugin-jest eslint-plugin-node eslint-plugin-promise eslint-plugin-standard -D
# package.json
"eslintConfig": {
    "extends": [
      "standard",
      "plugin:jest/recommended"
    ]
  }
```