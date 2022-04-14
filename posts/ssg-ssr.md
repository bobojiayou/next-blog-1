---
title: '杨波之，next如何处理静态资源、元数据、样式'
date: '2020-01-02'
---

### 静态资源、元数据、样式 
- 如何将静态文件（图像等）添加到 Next.js？
Next.js 可以在顶级公共目录下提供静态文件，如图像。 public 中的文件可以从应用程序的根目录中引用
eg. 如果你需要在pages/index.js中引入一个图片img1.png, 那你的引入路径是 /img1.png
- 如何自定义每个页面的 <head> 中的内容
next.js 首页中用的next.js内置组件 <Head>，而不是html标签<head>，可以直接在代码中，在<Head>  组件中添加自己的 title 
如果要自定义 <html>，例如添加 lang 属性，可以通过创建 pages/_document.js 文件来实现
- 如何创建一个使用 CSS 模块样式化的可重用 React 组件
Next 用的是名为 styled-jsx 的库。它是一个“CSS-in-JS”库——它允许您在 React 组件中编写 CSS，并且 CSS 样式将被限定
Next.js 内置了对 styled-jsx 的支持，但您也可以使用其他流行的 CSS-in-JS 库，例如 styled-components 或 Emotion
- 如何编写与导出样式文件
示例代码TODO