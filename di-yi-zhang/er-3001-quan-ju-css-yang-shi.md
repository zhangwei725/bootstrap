# 全局CSS样式

## 一、布局容器

### 1、概要

> Bootstrap 需要为页面内容和栅格系统包裹一个 .container 容器。我们提供了两个作此用处的类。
>
> 注意，由于 padding 等属性的原因，这两种 容器类不能互相嵌套。

### 2、container

1. 说明

   用于固定宽度并支持响应式布局的容器。

2. 示例代码

   ```
   <div class="container"> ...</div>
   ```

### 3、container-fluid

1. 说明

   用于 100% 宽度，占据全部视口（viewport）的容器

2. 示例代码

   ```
   <div class="container-fluid">...</div>
   ```

### 4、注意

> 这两个class不能放在一起，可以是兄弟关系，但不能是嵌套的关系。如果不想让宽度随着屏幕而变化，可以给它一个!important来提升优先级，这样的话在所有尺寸下都是一个定值

## 二、栅格系统

### 1、概要

Bootstrap 提供了一套响应式、移动设备优先的流式栅格系统，随着屏幕或视口（viewport）尺寸的增加，系统会自动分为最多12列。

### 2、工作原理

> 栅格系统用于通过一系列的行（row）与列（column）的组合来创建页面布局，你的内容就可以放入这些创建好的布局中。下面就介绍一下 Bootstrap 栅格系统的工作原理
>
> 1. “行（row）”必须包含在 `.container` （固定宽度）或 `.container-fluid` （100% 宽度）中，以便为其赋予合适的排列（aligment）和内补（padding）。
> 2. 通过“行（row）”在水平方向创建一组“列（column）”。
> 3. 你的内容应当放置于“列（column）”内，并且，只有“列（column）”可以作为行（row）”的直接子元素。
> 4. 类似 `.row` 和 `.col-xs-4` 这种预定义的类，可以用来快速创建栅格布局。Bootstrap 源码中定义的 mixin 也可以用来创建语义化的布局。
> 5. 通过为“列（column）”设置 `padding` 属性，从而创建列与列之间的间隔（gutter）。通过为 `.row` 元素设置负值 `margin` 从而抵消掉为 `.container` 元素设置的 `padding`，也就间接为“行（row）”所包含的“列（column）”抵消掉了`padding`。
> 6. 负值的 margin就是下面的示例为什么是向外突出的原因。在栅格列中的内容排成一行。
> 7. 栅格系统中的列是通过指定1到12的值来表示其跨越的范围。例如，三个等宽的列可以使用三个 `.col-xs-4` 来创建。
> 8. 如果一“行（row）”中包含了的“列（column）”大于 12，多余的“列（column）”所在的元素将被作为一个整体另起一行排列。
> 9. 栅格类适用于与屏幕宽度大于或等于分界点大小的设备 ， 并且针对小屏幕设备覆盖栅格类。 因此，在元素上应用任何 `.col-md-*` 栅格类适用于与屏幕宽度大于或等于分界点大小的设备 ， 并且针对小屏幕设备覆盖栅格类。 因此，在元素上应用任何 `.col-lg-*` 不存在， 也影响大屏幕设备

### 3、常用样式

1. lg: 宽度&gt;1200px

   > 屏幕的宽度大于1200，一行显示n\(结构里有几个div\)列屏幕的宽度小于1200，一行显示1列

2. md: 992px &lt;= 宽度 &lt;= 1200px

   > 屏幕的宽度大于992并且小于1200，一行显示n\(结构里有几个div\)列屏幕的宽度小于992，一行显示1列

3. sm: 768px &lt;= 宽度 &lt;= 992px

   > 屏幕的宽度大于768并且小于992，一行显示n\(结构里有几个div\)列屏幕的宽度小于768，一行显示1列

4. xs: 宽度 &lt;= 768px

   > 屏幕的宽度小于768，一行永远显示n\(结构里有几个div\)列

   **总结**

   lg ，md，sm，xs

5. col-\*-offset-\*\(列偏移\)

   > 向右偏移，第一个 _ 是和屏幕尺寸有关，第二个 _ 是偏移的列数，如果偏移的数量大于12则会不起作用

6. col-\*-push-\*\(列排序\)

   ```
   col--push（pull）- 第一个 * 是和屏幕尺寸有关，第二个 * 是往右或者往左的列数，不能超过12，否则就不起作用，push是往右推，pull是往左拉
   ```

   **区别**

   * 列偏移只能往右走，而列排序（pull、push）既可以往右边走，也可以往左边走
   * 如果一行中有多列，offset偏移如果大的话，会换行再偏移，而push不会有这个问题，可以溢出父级的容器。

### 4、示例代码

1. 基础使用

   ```
      <!--col-lg-*-->
           <div class="row">
               <div class="col-lg-12">第一行</div>
           </div>
           <!--col-lg-*-->
           <div class="row">
               <div class="col-lg-6">第2行第1列</div>
               <div class="col-lg-6">第2行第2列</div>
           </div>
           <!--col-md-*-->
           <div class="row">
               <div class="col-md-4">第3行第1列</div>
               <div class="col-md-4">第3行第2列</div>
               <div class="col-md-4">第3行第3列</div>
           </div>
           <!--col-sm-*-->
           <div class="row">
               <div class="col-sm-4">第4行第1列</div>
               <div class="col-sm-4">第4行第2列</div>
               <div class="col-sm-4">第4行第3列</div>
           </div>
           <!--col-xs-*-->
           <div class="row">
               <div class="col-xs-3">第5行第1列</div>
               <div class="col-xs-3">第5行第2列</div>
               <div class="col-xs-3">第5行第3列</div>
               <div class="col-xs-3">第5行第4列</div>
           </div>
       </div>
   ```

2. 组合使用

   ```
   <div class="container">
     <div class="row">
       <div class="col-lg-3">第1行第1列</div>
     </div>
     <div class="row">
       <div class="col-lg-3 col-md-4 col-sm-6">第1行第1列</div>
       <div class="col-lg-3 col-md-4 col-sm-6">第1行第2列</div>
       <div class="col-lg-3 col-md-4 col-sm-6">第1行第3列</div>
       <div class="col-lg-3 col-md-4 col-sm-6">第1行第4列</div>
     </div>

   </div>
   ```

3. 列偏移

   ```
   <div class="container">
     <div class="row">
       <div class="col-lg-3 col-md-4 col-sm-6">第1行第1列</div>
       <div class="col-lg-3 col-md-4 col-sm-6">第1行第2列</div>
       <div class="col-lg-3 col-md-4 col-sm-6">第1行第3列</div>
       <div class="col-lg-3 col-md-4 col-sm-6">第1行第4列</div>
     </div>
     <div class="row">
       <div class="col-lg-3">第1行第1列</div>
     </div>
   </div>
   ```

4. 列排序

   ```
   <style>
     .row div{
       background: green;
       color: #fff;
       border: 1px solid #000;
     }
   </style>

   <div class="container" style="border: 1px solid #f00;">
     <div class="row">
       <div class="col-lg-2 col-lg-push-5">第1行第1列</div>
       <div class="col-lg-2 col-lg-push-13">第1行第2列</div>
     </div>

     <div class="row">
       <div class="col-lg-2 col-lg-pull-1">第2行第1列</div>
       <div class="col-lg-2 col-lg-pull-13">第2行第2列</div>
     </div>
     <div class="row">
       <div class="col-lg-2 col-lg-push-10">第3行第1列</div>
       <div class="col-lg-10 col-lg-pull-2">第3行第2列</div>
     </div>
   </div>
   ```

   ​

5. 嵌套

   ```
   <style>
     .row div{
       background: green;
       color: #fff;
       border: 1px solid #000;
     }
   </style>

   <div class="container">
       <div class="row">
           <div class="col-lg-6">
               <!--第1行第1列-->
               <div class="row">
                   <div class="col-lg-4"></div>
                   <div class="col-lg-4"></div>
                   <div class="col-lg-4"></div>
               </div>
           </div>
           <div class="col-lg-6">第1行第2列</div>
       </div>
   </div>
   ```

   ​



