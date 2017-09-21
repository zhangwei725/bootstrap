# 标签和样式(一)

## 一、基础标签

### 1、说明

> Bootstrap 中把一些标签的样式重置了，也即是为一些标签设置了带有 Bootstrap 风格的样式，如 h 标签，p 标签等等，这其中包含了 HTML5 标签

### 2、head标签、内联子标题

1. 说明

   > Bootstrap 中定义了所有的 HTML 标题（h1 到 h6）的样式
   > 向任何标题添加一个内联子标题，只需要简单地在元素两旁添加 \<small>，或者添加 .small class，这样子您就能得到一个字号更小的颜色更浅的文本


1. 示例代码

   ```
   <span class="h1">我是标题1 h1: <small>我是副标题1 h1</small></span>
   <span class="h2">我是标题2 h2: <span class="small">我是副标题2 h2</small></span>
   <span class="h3">我是标题3 h3:<small>我是副标题3 h3</small></span>
   <span class="h4">我是标题4 h4: <small>我是副标题4 h4</small></span>
   <span class="h5">我是标题5 h5: <small>我是副标题5 h5</small></span>
   <span class="h6">我是标题6 h6: <small>我是副标题6 h6</small></span>
   ```

### 3、文本样式

#### 3.1、属性介绍

1. text-left

   向左对齐文本

2. text-center

   居中对齐文本

3. text-right

   向右对齐文本

4. text-muted

   本行内容是减弱的

5. text-primary

   本行内容带有一个 primary class

6. text-success

   本行内容带有一个success class

7. text-info

   本行内容带有一个 info class

8. text-warning

   本行内容带有一个 warning class

9. text-danger

   本行内容带有一个 danger class

#### 3.2、示例代码

1. 示例一

   ```
   <p class="text-left">向左对齐文本</p>
   <p class="text-center">居中对齐文本</p>
   <p class="text-right">向右对齐文本</p>
   <p class="text-muted">本行内容是减弱的</p>
   <p class="text-primary">本行内容带有一个 primary class</p>
   <p class="text-success">本行内容带有一个 success class</p>
   <p class="text-info">本行内容带有一个 info class</p>
   <p class="text-warning">本行内容带有一个 warning class</p>
   <p class="text-danger">本行内容带有一个 danger class</p>
   ```

### 4、其它标签

#### 4.1、属性介绍

1. initialism

   缩写,HTML 元素提供了用于缩写的标记，比如 WWW 或 HTTP

2. address

   使用 \<address> 标签，您可以在网页上显示联系信息。由于 \<address> 默认为 display:block;，您需要使用 
   标签来为封闭的地址文本添加换行

#### 4.2、示例代码

1. 示例一

   ```
   <abbr title="World Wide Web">WWW</abbr><br>
   ```

2. 示例代码

   ```
   <address>
     <strong>公司邮箱</strong><br>
     <a href="">123@163.com</a>
   </address>
   ```

## 二、表格

### 1、说明

> bootstrap 也重置了表格这个标签，加入了表格常用的样式，比如隔行换色，加边框等，下面是 Bootstrap 的表格类名，它们可以组合使用	

### 2、属性说明

#### 2.1、表格属性

1. table

   > 添加基本样式 

2. table-striped

   > 隔行换色

3. table-bordered

   > 给表格添加边框

4. table-hover

   > 给每一行添加一个hover状态

5. table-condensed

   > 让表格更加紧凑

6. .table-striped

#### 2.2、行或者单元格

1. active

   > 鼠标悬停在行或单元格上时所设置的颜色

2. success

   > 标识成功或积极的动作

3. info

   > 标识普通的提示信息或动作

4. warning

   > 标识警告或需要用户注意

5. danger

   > 标识危险或潜在的带来负面影响的动作

### 3、示例代码

1. 表格基本操作

   ```
       <div class="row">
           <table class="table table-bordered table-condensed table-hover table-responsive" >
               <tr>
                   <th>ID</th>
                   <th>用户名</th>
                   <th>性别</th>
                   <th>手机</th>
                   <th>邮箱</th>
                   <th>地址</th>
                   <th>加入时间</th>
                   <th>状态</th>
               </tr>
               <tr class="success">
                   <td>1</td>
                   <td>老王</td>
                   <td>男</td>
                   <td>110</td>
                   <td>123@163.com</td>
                   <td>三里屯</td>
                   <td>2017-10-25</td>
                   <td>激活</td>
               </tr>
               <tr class="warning">
                   <td>1</td>
                   <td>老王</td>
                   <td>男</td>
                   <td>110</td>
                   <td>123@163.com</td>
                   <td>三里屯</td>
                   <td>2017-10-25</td>
                   <td>激活</td>
               </tr>
               <tr class="danger">
                   <td>1</td>
                   <td>老王</td>
                   <td>男</td>
                   <td>110</td>
                   <td>123@163.com</td>
                   <td>三里屯</td>
                   <td>2017-10-25</td>
                   <td>激活</td>
               </tr>
               <tr class="info">
                   <td>1</td>
                   <td>老王</td>
                   <td>男</td>
                   <td>110</td>
                   <td>123@163.com</td>
                   <td>三里屯</td>
                   <td>2017-10-25</td>
                   <td>激活</td>
               </tr>
               <tr>
                   <td>1</td>
                   <td>老王</td>
                   <td>男</td>
                   <td>110</td>
                   <td>123@163.com</td>
                   <td>三里屯</td>
                   <td>2017-10-25</td>
                   <td>激活</td>
               </tr>
           </table>
       </div
   </div>
   ```

2. 样式操作

   ```
     <table class="table" >
               <tr>
                   <th>ID</th>
                   <th>用户名</th>
                   <th>性别</th>
                   <th>手机</th>
                   <th>邮箱</th>
                   <th>地址</th>
                   <th>加入时间</th>
                   <th>状态</th>
               </tr>
               <tr >
                   <td>1</td>
                   <td>老王</td>
                   <td>男</td>
                   <td>110</td>
                   <td>123@163.com</td>
                   <td>三里屯</td>
                   <td>2017-10-25</td>
                   <td>激活</td>
               </tr>
               <tr>
                   <td>1</td>
                   <td>老王</td>
                   <td>男</td>
                   <td>110</td>
                   <td>123@163.com</td>
                   <td>三里屯</td>
                   <td>2017-10-25</td>
                   <td>激活</td>
               </tr>
               <tr>
                   <td>1</td>
                   <td>老王</td>
                   <td>男</td>
                   <td>110</td>
                   <td>123@163.com</td>
                   <td>三里屯</td>
                   <td>2017-10-25</td>
                   <td>激活</td>
               </tr>
               <tr>
                   <td>1</td>
                   <td>老王</td>
                   <td>男</td>
                   <td>110</td>
                   <td>123@163.com</td>
                   <td>三里屯</td>
                   <td>2017-10-25</td>
                   <td>激活</td>
               </tr>
               <tr>
                   <td>1</td>
                   <td>老王</td>
                   <td>男</td>
                   <td>110</td>
                   <td>123@163.com</td>
                   <td>三里屯</td>
                   <td>2017-10-25</td>
                   <td>激活</td>
               </tr>
     </table>
   ```

## 三、表单

### 1、概要

> Bootstrap 提供了下列类型的表单布局
>
> 1. 垂直表单（默认）
> 2. 内联表单
> 3. 水平表单

### 2、基本样式

#### 2.1、作用

> 单独的表单控件会被自动赋予一些全局样式。所有设置了 `.form-control` 类的 `<input>`、`<textarea>` 和 `<select>` 元素都将被默认设置宽度属性为 `width: 100%;`。 将 `label` 元素和前面提到的控件包裹在 `.form-group` 中可以获得最好的排列

#### 2.2  示例代码

1. 示例一

   ```
   <form>
     <div class="form-group">
       <label for="name">用户名</label>
       <input type="text" class="form-control" id="name" placeholder="请输入用户名">
     </div>
     <div class="form-group">
       <label for="file">选择上传文件</label>
       <input type="file" id="file">
     </div>
     <div class="checkbox">
       <label>
         <input type="checkbox">请打勾
       </label>
     </div>
     <button type="submit">提交</button>
   </form>
   ```

### 3、内联表单

#### 3.1、说明

> 为 `<form>` 元素添加 `.form-inline` 类可使其内容左对齐并且表现为 `inline-block` 级别的控件。**只适用于视口（viewport）至少在 768px 宽度时（视口宽度再小的话就会使表单折叠）**

#### 3.2、注意事项

1. 可以手动设置宽度

   > 在 Bootstrap 中，输入框和单选/多选框控件默认被设置为 `width: 100%;` 宽度。在内联表单，我们将这些元素的宽度设置为 `width: auto;`，因此，多个控件可以排列在同一行。根据你的布局需求，可能需要一些额外的定制化组件。

2. 一定要添加 `label` 标签

   > 如果你没有为每个输入控件设置 `label` 标签，屏幕阅读器将无法正确识别。对于这些内联表单，你可以通过为 `label` 设置 `.sr-only` 类将其隐藏。还有一些辅助技术提供label标签的替代方案，比如 `aria-label`、`aria-labelledby` 或 `title` 属性。如果这些都不存在，屏幕阅读器可能会采取使用 `placeholder` 属性，如果存在的话，使用占位符来替代其他的标记

#### 3.3、示例代码

1. 示例一

   ```
    <form class="form-inline">
           <div class="form-group">
               <label for="name">用户名</label>
               <input type="text" class="form-control" id="username" placeholder="请输入用户名">
           </div>
           <div class="form-group">
               <label for="name">设置密码</label>
               <input type="text" class="form-control" id="pwd" placeholder="请输入密码">
           </div>
    
           <div class="form-group">
               <label for="name">确认密码</label>
               <input type="text" class="form-control" id="pwd1" placeholder="请确认密码">
           </div>
           <div class="form-group">
               <label for="email">邮箱</label>
               <input type="email" class="form-control" id="email" placeholder="123456@example.com">
           </div>
           <button type="submit">注册</button>
       </form>
   </div>
   ```

### 4、水平排列的表单

#### 1、说明

> 通过为表单添加 `.form-horizontal` 类，并联合使用 Bootstrap 预置的栅格类，可以将 `label` 标签和控件组水平并排布局。这样做将改变 `.form-group` 的行为，使其表现为栅格系统中的行（row），因此就无需再额外添加 `.row` 了

#### 2、示例代码

1. 示例一

   ```
     <span class="h1">水平排列</span>

       <form class="form-horizontal">

           <div class="form-group">
               <label for="uname" class="col-sm-2 control-label">用户名</label>
               <div class="col-sm-10">
                   <input type="text" class="form-control" id="uname" placeholder="请输入用户名">
               </div>
           </div>
           <div class="form-group">
               <label for="password" class="col-sm-2 control-label">密码</label>
               <div class="col-sm-10">
                   <input type="password" class="form-control" id="password" placeholder="请输入密码">
               </div>
           </div>
    
           <div class="form-group">
               <div class="col-sm-offset-2 col-sm-10 checkbox">
                   <label>
                       <input type="checkbox">记住密码
                   </label>
               </div>
           </div>
           <div class="form-group">
               <div class="col-sm-offset-2 col-sm-10">
                   <button type="submit" class="btn">登录</button>
               </div>
           </div>
       </form>
   ```

#### 5、多选和单选框

#### 5.1 、说明

> 多选框（checkbox）用于选择列表中的一个或多个选项，而单选框（radio）用于从多个选项中只选择一个

#### 5.2 、示例代码

1. 示例一(默认外观,堆叠在一起)

   ```
     <h1>多选单选</h1>
       <div class="checkbox">
           <label>
               <input type="checkbox" value="1">
               多选
           </label>
       </div>
       <div class="checkbox disabled">
           <label>
               <input type="checkbox" value="2" disabled>
               不可操作
           </label>
       </div>
       <div class="radio">
           <label>
               <input type="radio" name="r1" id="rid1" value="o1" checked>
               单选默认选中
           </label>
       </div>
       <div class="radio">
           <label>
               <input type="radio" name="r1" id="rid2" value="o2">
               妹子1
           </label>
       </div>
       <div class="radio disabled">
           <label>
               <input type="radio" name="r1" id="rid3" value="3" disabled>
               妹子2
           </label>
       </div>
   </div>
   ```

2. 示例二(内联单选和多选框)

   ```
    <!--通过将 .checkbox-inline
       或 .radio-inline 类应用到一系列的多选框（checkbox）
       或单选框（radio）控件上，可以使这些控件排列在一行。-->

       <label class="checkbox-inline">
           <input type="checkbox" id="ick1" value="v1">1
       </label>
       <label class="checkbox-inline">
           <input type="checkbox" id="ick2" value="v2">2
       </label>
       <label class="checkbox-inline">
           <input type="checkbox" id="ick3" value="v3">3
       </label>

       <label class="radio-inline">
           <input type="radio" name="ri" id="ri1" value="v1">1
       </label>
       <label class="radio-inline">
           <input type="radio" name="ri" id="ri2" value="v2">2
       </label>
       <label class="radio-inline">
           <input type="radio" name="ri" id="ri3" value="v3">3
       </label>
   </div>
   ```

3. 下拉列表

   ```
   <select class="form-control">
     <option>1</option>
     <option>2</option>
     <option>3</option>
     <option>4</option>
     <option>5</option>
   </select>
   <select multiple class="form-control">
     <option>1</option>
     <option>2</option>
     <option>3</option>
     <option>4</option>
     <option>5</option>
   </select>
   ```

#### 5.3、其它常用属性

1. has-warning 表单填写警告
2. has-error 表单填写错误
3. has-success 表单填写成功

## 四、按钮

### 1、说明

> 可作为按钮使用的标签或元素
>
> `<a>`、`<button>` 或 `<input>` 元素添加按钮类（button class）即可使用 Bootstrap 提供的样式。

### 2、属性

#### 2.1、背景色

1. btn-default 默认的按钮样式
2. btn-link 链接样式的按钮
3. btn-primary 首选项颜色的按钮
4. btn-success 成功颜色的按钮
5. btn-info 一般信息颜色的按钮
6. btn-warning 警告颜色的按钮
7. btn-danger 危险颜色的按钮

#### 2.2、按钮的尺寸

1. btn-lg 
2. btn-md 
3. btn-sm 
4. btn-xs

#### 2.3、状态

1. active（激活状态）
2. disabled（禁用状态）

#### 2.4、状态

1. btn-block 

   让按钮从内联块级元素变为块级元素，

   可以撑满整个父级元素，也即是把按钮的宽度置为100%；

### 3、示例代码

1. 基础按钮

   ```
   <div class="container">
       <div class="row">
           <input type="button" value="按钮" class="btn" />
           <button type="button" class="btn btn-default">按钮</button>
           <button type="button" class="btn btn-primary">按钮</button>
           <button type="button" class="btn btn-success">按钮</button>
           <button type="button" class="btn btn-info">按钮</button>
           <button type="button" class="btn btn-warning">按钮</button>
           <button type="button" class="btn btn-danger">按钮</button>
           <button type="button" class="btn btn-link">按钮</button>
       </div>
   </div>
   ```

2. 按钮尺寸

   ```
   <div class="container">
       <!--按钮的尺寸-->
       <div class="row" style="margin-top: 10px;">
           <button type="button" class="btn btn-default btn-lg">按钮</button>
           <button type="button" class="btn btn-primary btn-md">按钮</button>
           <button type="button" class="btn btn-success btn-sm">按钮</button>
           <button type="button" class="btn btn-info btn-xs">按钮</button>
       </div>
   </div>
   ```

3. 块级按钮

   ```
   <div class="container">
     <div class="row"">
           <button type="button" class="btn btn-primary btn-block">按钮</button>
    </div>
   </div>
   ```

4. 激活状态

   ```
   <!--激活状态-->
   <div class="row">
           <button type="button" class="btn btn-primary active">按钮</button>
           <a href="#" class="btn btn-danger active">按钮</a>
   </div>
   ```

5. 禁用状态

   ```
    <!--禁用状态-->
       <div class="row">
           <button type="button" class="btn btn-primary active" disabled>按钮</button>
           <button type="button" class="btn btn-info disabled">按钮</button>
       </div>
   ```

6. 链接按钮