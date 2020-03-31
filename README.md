# tiny-wheels
一套基于原生JavaScript开发的组件库，无依赖、体积小、简单易用

<!-- ## 文档 -->

<!-- 关于各个组件的详细使用方式可以查看本项目的文档： -->

## 特性

- 使用`ES6`最新语法编写，纯原生`JavaScript`代码，适合新手阅读
- 无任何第三方依赖，源码非常精简，可以自由拓展组件功能
- 基于`Webpack`和`Babel`的最新版本构建，采用`UMD`的模块化规范打包，兼容多种引入方式

## 使用

- 模块化引入（推荐）

> npm install tiny-wheels -D

```javascript
import { Tabs } from 'tiny-wheels'

new Tabs(document.querySelector('.tabs'))
```

- 标签引入

目前可以通过[unpkg.com/tiny-wheels](https://unpkg.com/tiny-wheels/dist/index.js)获取到最新版本的资源，在页面上使用script标签引入后即可开始使用

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Example</title>
</head>
<body>
    <script src="https://unpkg.com/tiny-wheels/dist/index.js"></script>
    <script>
        new TinyWheels.Tabs(document.querySelector('.tabs'))
    </script>
</body>
</html>
```

由于项目已经暴露了全局变量`TinyWheels`，所以在浏览器环境可以直接使用，通过标签引入的具体示例可以参考项目根目录下的`example.html`

## 开发

此项目为个人项目，非常欢迎大家下载本项目自由开发，如果有优秀的组件提交，我会直接合并进项目中

### 运行

通过如下步骤可以直接运行项目：

1. git clone https://github.com/csdoker/tiny-wheels.git
2. npm install
3. npm run start
4. open localhost:8000

运行入口为`src/main.js`文件，该文件中是各个组件的使用代码，可以自由修改测试

### 打包

使用命令：

> npm run build

打包入口为`src/index.js`文件，目前的做法是在各个组件中引入了对应的样式，然后将所有组件导出为一个对象

## 进度

- [x] Tabs-选项卡
- [ ] Collapse-折叠面板
- [ ] Pager-分页
- [ ] Carousel-走马灯
- [ ] Calendar-日历
- [ ] 单元测试

持续施工中...

## 参考

[Element](https://element.eleme.cn/#/zh-CN)
[Ant Design](https://ant.design/)
[iView](https://www.iviewui.com/)
[wheels](https://github.com/FrankFang/wheels)
[qing](https://github.com/veedrin/qing)
[yu.js.ui](https://github.com/yurencloud/yu.js.ui/)
[xy-ui](https://github.com/XboxYan/xy-ui)
[gulu](https://github.com/FrankFang/gulu)