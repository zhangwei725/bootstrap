# BootStrap

## 一、概要

1. Bootstrap，来自 Twitter，是目前很受欢迎的前端框架。
2. 是一个用于快速开发 Web 应用程序和网站的前端框架。Bootstrap 是基于 HTML、CSS、JavaScript 的，它简洁灵活，使得 Web 开发更加快捷。
3. 它由Twitter的设计师Mark Otto和Jacob Thornton合作开发，是一个CSS/HTML框架。Bootstrap提供了优雅的HTML和CSS规范，它即是由动态CSS语言Less写成

## 二、组成

1. 栅格系统

   将屏幕平分12份（列）。使用行(row)来组织元素（每一行都包括12个列），然后将内容放在列内。通过col-md-offset-*来控制列偏移。

2. 基础布局组件

   Bootstrap提供了多种基础布局组件。如排版、代码、表格、按钮、表单等。

3. Jquery

   Bootstrap所有的JavaScript插件都依赖于Jquery的。如果要使用这些JS插件，就必须引用Jquery库。这也是为什么我们在除了要引用Bootstrap的JS文件和CSS文件外，还需要引用Jquery库的原因，两者是依赖关系。

4. CSS组件

   Bootstrap为我们预实现了很多CSS组件。如下拉框、按钮组、导航等。也就是说Bootstrap内容帮我们定义好了很多CSS样式，你可以将这些样式直接应用到之前的下拉框等元素里。

5. JavaScript插件

   Bootstrap也为我们实现了一些JS插件，我们可以用其提供的插件要完成一些常用功能，而不需要我们再重新写JS代码来实现像提示框，模态窗口这样的效果了。

6. 响应式设计

   响应式的意思就是它会根据屏幕尺寸来自动调整页面，使得前端页面在不同尺寸的屏幕上都可以表现很好。

## 三、基本模板

1. 核心包

   ```
     <head>
       <meta charset="utf-8">
       <!--开发版-->
       <link href="https://cdn.bootcss.com/bootstrap/3.3.7/css/bootstrap.css" rel="stylesheet">
       <!--上线版-->
       <link href="https://cdn.bootcss.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">
     </head>
   ```

2. 对jQuery支持

   ```
   <!--需要导入jQuery库-->
   <script src="https://cdn.bootcss.com/jquery/3.2.1/jquery.js"></script>
   <!--开发版-->
   <script src="https://cdn.bootcss.com/bootstrap/3.3.7/js/bootstrap.js"></script>
   <!--上线版-->
   <script src="https://cdn.bootcss.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
   ```

3. 让IE9以下的IE浏览器兼容新增的HTML5标签和CSS3样式

   ```
   <!--[if lt IE 9]>
   <script src="https://cdn.bootcss.com/html5shiv/3.7.3/html5shiv.min.js"></script>
   <script src="https://cdn.bootcss.com/respond.js/1.4.2/respond.min.js"></script>
   <![endif]-->
   ```

4. 主题

   ```
   <!--开发版-->
   <link href="https://cdn.bootcss.com/bootstrap/3.3.7/css/bootstrap-theme.css" rel="stylesheet">
   <!--上线版-->
   <link href="https://cdn.bootcss.com/bootstrap/3.3.7/css/bootstrap-theme.min.css" rel="stylesheet">
   ```

5. 为了增强跨浏览器表现的一致性,浏览器CSS 重置样式库

   ```
   <!--开发版-->
   <link href="https://cdn.bootcss.com/normalize/7.0.0/normalize.css" rel="stylesheet">
   <!--上线版-->
   <link href="https://cdn.bootcss.com/normalize/7.0.0/normalize.min.css" rel="stylesheet">
   ```

6. 其它

   ```
   <!-- 使IE浏览器用最新的edge引擎渲染页面 -->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!-- 让页面的最大宽度等于设备的宽度，页面初始化为不缩放状态，当然这样还是可以缩放的 -->
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <!-- 上述3个meta标签必须放在最前面，任何其他内容都必须跟随其后-->
   <!-- 使360浏览器渲染页面时默认使用极速模式 -->
   <meta name="renderer" content="webkit">
   ```

###  

