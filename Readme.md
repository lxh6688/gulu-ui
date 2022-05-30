# gulu-ui-by-vue - 一个 Vue UI 组件

作者： Lixiaohu

## 介绍

## 开始使用 

1. 安装
使用本框架前，请在 CSS 中开启 border-box

```
*, *::before, *::after{box-sizing: border-box}
```

IE 8 及以上浏览器都支持使用此样式

你还需要设置默认颜色等变量（后续会改为 SCSS 变量）
```
html {
  --button-height: 32px;
  --font-size: 14px;
  --button-bg: white;
  --button-active-bg: #eee;
  --border-radius: 4px;
  --color: #333;
  --border-color: #999;
  --border-color-hover: #666;
}
```

IE 15 及以上浏览器都支持使用此样式

2. 安装 gulu
```
npm i --save gulu-ui-by-vue
```

3. 引入
```
import {Button} from 'gulu-ui-by-vue'
import 'gulu-ui-by-vue/dist/index.css'
export default {
  name: 'App',
  components: {
    'g-button': Button
  }
}
```

## 文档

## 提问

## 变更记录

## 联系方式

## 贡献代码