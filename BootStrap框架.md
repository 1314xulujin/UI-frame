## 										BootStrap框架

> ​	来自 Twitter，是目前最受欢迎的前端框架。Bootstrap 是基于 HTML、CSS、JAVASCRIPT 的，它简洁灵活，使得 Web 开发更加快捷。基于H5标准 , 秉承移动端优先 构建移动端和PC响应式网站

###### 中文文档地址: <https://v3.bootcss.com/>

###### 布局容器:

​	.container   布局主要容器 , 跟以前的wrap一样的

​	.container-fluid	满屏的容器 , 用于 100% 宽度，占据全部视口（viewport）的容器

###### 框架默认主题风格颜色:

~~~
default  灰色

primary  蓝色

success  绿色

info     浅蓝色

warning  橙色

danger   红色
~~~

###### 状态样式类:

~~~
.active 激活
.success
.info
.danger
.warning

.disabled
~~~

###### 浮动类:

~~~
.clearfix 清除浮动
.pull-left 左浮动
.pull-right 右浮动

不能用于导航条组件中
排列导航条中的组件时可以使用这些工具类：.navbar-left 或 .navbar-right
~~~

###### 其他:

~~~
.center-block 块级元素居中

关闭按钮: <button class="close"><span>&times;</span></button>
三角符号: <span class="caret"></span>

显示 / 隐藏 : .show 和 .hidden 

图片替换: .text-hide  文字隐藏 ,只显示背景图片 
~~~

###### 栅格系统:一套响应式、移动设备优先的流式栅格系统，随着屏幕或视口（viewport）尺寸的增加，系统会自动分为最多12列

~~~
行 (.row)

列 (.col-*)
	按屏幕划分列名:
		.col-xs-1  .... -- .col-xs-12   (12个)
		.col-sm-1  .... -- .col-sm-12   (12个)
		.col-md-1  .... -- .col-md-12   (12个)
		.col-lg-1  .... -- .col-lg-12   (12个)

~~~

###### 屏幕种类划分:

通过下表可以详细查看 Bootstrap 的栅格系统是如何在多种屏幕设备上工作的。

|                       | 超小屏幕 手机 (<768px)  xs | 小屏幕 平板 (≥768px) sm                             | 中等屏幕 桌面显示器 (≥992px) md | 大屏幕 大桌面显示器 (≥1200px)  lg |
| :-------------------- | :------------------------- | :-------------------------------------------------- | :------------------------------ | :-------------------------------- |
| 栅格系统行为          | 总是水平排列               | 开始是堆叠在一起的，当大于这些阈值时将变为水平排列C |                                 |                                   |
| `.container` 最大宽度 | None （自动）              | 750px                                               | 970px                           | 1170px                            |
| 类前缀                | `.col-xs-`                 | `.col-sm-`                                          | `.col-md-`                      | `.col-lg-`                        |
| 列（column）数        | 12                         |                                                     |                                 |                                   |
| 最大列（column）宽    | 自动                       | ~62px                                               | ~81px                           | ~97px                             |
| 槽（gutter）宽        | 30px （每列左右均有 15px） |                                                     |                                 |                                   |
| 可嵌套                | 是                         |                                                     |                                 |                                   |
| 偏移（Offsets）       | 是                         |                                                     |                                 |                                   |
| 列排序                | 是                         |                                                     |                                 |                                   |

###### 列偏移(48个):

~~~
.col-xs-offset-1  --  .col-xs-offset-12
.col-sm-offset-1  --  .col-sm-offset-12
.col-md-offset-1  --  .col-md-offset-12
.col-lg-offset-1  --  .col-lg-offset-12
~~~

###### 列排序(96个):

~~~
col-*-push-*:  48个
col-*-pull-*:  48个
~~~

---

#### 排版

###### 1.重写标题标签样式 , 浏览器常见标签的默认样式重置

###### 2.文本样式(text):

~~~
对齐:
.text-left  文本左对齐
.text-center  居中
.text-right   右对齐
.text-justify 两端对齐
.text-nowrap   不换行

改变大小写:
.text-lowercase  文本小写
.text-uppercase  大写
.text-capitalize  首字母大写

文本颜色:
.text-primary 
.text-info
.text-success
.text-warning
.text-danger

背景色:
.bg-primary 
.bg-info
.bg-success
.bg-warning
.bg-danger
~~~

###### 3.列表

~~~
.list-unstyled  无列表样式
.list-inline  行内列表
.dl-horizontal  水平排列的自定义列表
~~~

###### 4.表格(table)

~~~
.table   表格的基础样式类
.table-bordered 带边框
.table-hover   鼠标悬停背景色变化
.table-striped  条纹背景色
.table-condensed 紧凑表格

.table-responsive 响应式表格 , 需要把这个给到嵌套表格的div 即可
~~~

###### 5.表单

~~~
form:
.form-horizontal水平表单
.form-inline 内敛表单


.form-group 表单组 (包裹label 和 input)
.form-control  一般是给表单元素添加(input select textarea)
.control-label 给label设置的

表单的校验状态:
	每项表单组验证状态: .has-success / .has-warning  / .has-error
	
	带图标:
		每项表单组.has-feedback
		.form-control-feedback
		
~~~

###### 6.按钮: 为 `<a>`、`<button>` 或 `<input>` 元素添加按钮类（button class）即可使用 Bootstrap 提供的样式

~~~
.btn 

按钮颜色:
	.btn-primary
	.btn-success
	.btn-info
	.btn-warning
	.btn-danger
	.btn-link
	.btn-default

按钮大小:
	.btn-xs
	.btn-sm
	.btn-lg

按钮组(.btn-group):

块级按钮:.btn-block


~~~

###### 7.响应式工具: (处理移动屏幕元素内容选择性可见)

通过单独或联合使用以下列出的类，可以针对不同屏幕尺寸隐藏或显示页面内容。

|                 | 超小屏幕手机 (<768px) | 小屏幕平板 (≥768px) | 中等屏幕桌面 (≥992px) | 大屏幕桌面 (≥1200px) |
| :-------------- | :-------------------- | :------------------ | :-------------------- | :------------------- |
| `.visible-xs-*` | 可见                  | 隐藏                | 隐藏                  | 隐藏                 |
| `.visible-sm-*` | 隐藏                  | 可见                | 隐藏                  | 隐藏                 |
| `.visible-md-*` | 隐藏                  | 隐藏                | 可见                  | 隐藏                 |
| `.visible-lg-*` | 隐藏                  | 隐藏                | 隐藏                  | 可见                 |
| `.hidden-xs`    | 隐藏                  | 可见                | 可见                  | 可见                 |
| `.hidden-sm`    | 可见                  | 隐藏                | 可见                  | 可见                 |
| `.hidden-md`    | 可见                  | 可见                | 隐藏                  | 可见                 |
| `.hidden-lg`    | 可见                  | 可见                | 可见                  | 隐藏                 |

##### 注释: * 代表显示的类型: inline / inline-block / block

---

###### 8.打印类:

和常规的响应式类一样，使用下面的类可以针对打印机隐藏或显示某些内容。

| class                                                        | 浏览器 | 打印机 |
| :----------------------------------------------------------- | :----- | :----- |
| `.visible-print-block` `.visible-print-inline` `.visible-print-inline-block` | 隐藏   | 可见   |
| `.hidden-print`                                              | 可见   | 隐藏   |

`.visible-print` 类也是存在的，但是从 v3.2.0 版本开始**不建议使用**。它与 `.visible-print-block` 类大致相同，除了 `<table>` 相关元素的特殊情况外。

---

###### 1.下拉菜单组件  (dropdown)

~~~html
<div class="dropdown">
            <button class="btn btn-success" data-toggle="dropdown">下拉菜单</button>
            <ul class="dropdown-menu dropdown-menu-right">
                <li class="dropdown-header">Dropdown header</li>
                <li><a href="">二级菜单1</a></li>
                <li><a href="">二级菜单2</a></li>
                <li class="divider"></li>
                <li><a href="">二级菜单3</a></li>
                <li><a href="">二级菜单4</a></li>
                <li><a href="">二级菜单5</a></li>
            </ul>
        </div>
~~~

###### 2.输入框组(input-group)

~~~html
<div class="input-group">
            <label class="input-group-addon">商品</label>
            <input type="text" class="form-control">
</div>
~~~

###### 3.导航(nav):

~~~
nav
~~~

###### 4.导航条(navbar)

~~~html
.navbar   (.navbar-default 默认灰色背景)
.navbar-fixed-top 固定在顶部 
.navbar-fixed-bottom 固定在底部
.navbar-inverse 反色导航(黑色)
 
 导航条中的导航 (需要折叠展开: 使用.collapse.navbar-collapse 父级包裹)
 .nav.navbar-nav
 
 导航条的表单
 .navbar-form
 
 汉堡按钮
 <button class="navbar-toggle">
                <span class="icon-bar"></span>
                <span class="icon-bar"></span>
                <span class="icon-bar"></span>
</button>
汉堡按钮功能 : 
	data-toggle="collapse"   设置按钮的开关功能, 调用collapse插件
	data-traget=".navbar-collapse" 设置触发的目标元素 ,用于折叠对象

~~~

###### 5.进度条(progress)

~~~

~~~

