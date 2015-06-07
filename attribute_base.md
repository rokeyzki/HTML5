# 全局属性
这里列出的属性是通用于每个标签的核心属性和语言属性
***

## class 属性
> ### 说明：
* class 属性规定元素的类名
* class 属性大多数时候用于指向样式表中的类
* class 属性不能在以下 HTML 元素中使用：base, head, html, meta, param, script, style 以及 title
* 可以给 HTML 元素赋予多个 class
* 类名不能以数字开头

> ### 示例：
```html
<head>
    <style type="text/css">
        .intro {color:blue;}
        .important {color:green;}
    </style>
</head>
<body>
    <h1 class="intro">Header 1</h1>
    <p>A paragraph.</p>
    <p class="important">Note that this is an important paragraph.</p>
</body>
```

> ### 支持：
* 不支持的元素：`<base>` `<head>` `<html>` `<meta>` `<param>` `<script>` `<style>` `<title>`
* 不支持的浏览器：无

## dir 属性
> ### 说明：
* dir 属性规定元素内容的文本方向
* ltr值，表示从左向右的文本方向
* rtl值，表示从右向左的文本方向

> ### 示例：
```html
<body>
    <p dir="rtl">Write this text right-to-left!</p>
</body>
```

> ### 支持：
* 不支持的元素：`<base>` `<br>` `<frame>` `<frameset>` `<hr>` `<iframe>` `<param>` `<script>`
* 不支持的浏览器：无

## id 属性
> ### 说明：
* id 属性规定 HTML 元素的唯一的 id
* id 在 HTML 文档中必须是唯一的
* id 属性可用作链接锚

> ### 示例：
```html
<head>
    <script>
    function change_header(){
        document.getElementById("myHeader").innerHTML="Nice day!";
    }
    </script>
</head>
<body>
    <h1 id="myHeader">Hello World!</h1>
    <button onclick="change_header()">Change text</button>
</body>
```

> ### 支持：
* 不支持的元素：无
* 不支持的浏览器：无

## lang 属性
> ### 说明：
* lang 属性规定元素内容的语言

> ### 示例：
```html
<body>
    <p>This is a paragraph.</p>
    <p lang="fr">Ceci est un paragraphe.</p>
</body>
```

> ### 支持：
* 不支持的元素：`<base>` `<br>` `<frame>` `<frameset>` ` <hr>` `<iframe>` `<param>` `<script>`
* 不支持的浏览器：无

## style 属性
> ### 说明：
* style 属性规定元素的行内样式
* style 属性将覆盖任何全局的样式设定

> ### 示例：
```html
<body>
    <h1 style="color:blue;text-align:center">This is a header</h1>
    <p style="color:red">This is a paragraph.</p>
</body>
```

> ### 支持：
* 不支持的元素：无
* 不支持的浏览器：无

## tabindex 属性
> ### 说明：
* tabindex 属性规定元素的 tab 键控制次序（当 tab 键用于导航时）
* 规定元素的 tab 键控制次序（1 是第一个）

> ### 示例：
```html
<body>
    <a href="http://www.w3school.com.cn/" tabindex="2">W3School</a><br />
    <a href="http://www.google.com/" tabindex="1">Google</a><br />
    <a href="http://www.microsoft.com/" tabindex="3">Microsoft</a>
    <p><b>注释：</b>请尝试使用键盘上的 "Tab" 键在链接之间进行导航。</p>
</body>
```

> ### 支持：
* 支持的元素：`<a>` `<area>` `<button>` `<input>` `<object>` `<select>` `<textarea>`
* 不支持的浏览器：Safari

## title 属性
> ### 说明：
* title 属性规定关于元素的额外信息
* 这些信息通常会在鼠标移到元素上时显示一段工具提示文本（tooltip text）

> ### 示例：
```html
<body>
    <abbr title="People's Republic of China">PRC</abbr> was founded in 1949.
    <p title="Free Web tutorials">W3School.com.cn</p>
</body>
```

> ### 支持：
* 不支持的元素：无
* 不支持的浏览器：无

## contenteditable 属性 ※
> ### 说明：
* contenteditable 属性规定元素内容是否可编辑
* 如果元素未设置 contenteditable 属性，那么元素会从其父元素继承该属性
* true值，表示元素可编辑
* false值，表示元素不可编辑

> ### 示例：
```html
<body>
    <p contenteditable="true">这是一段可编辑的段落。请试着编辑该文本。</p>
</body>
```

> ### 支持：
* 不支持的元素：无
* 不支持的浏览器：IE9 -

## contentextmenu 属性 ※
> ### 说明：
* 规定元素的上下文菜单
* 上下文菜单会在用户右键点击元素时出现
* contextmenu 属性的值是要打开的 <menu> 元素的 id

> ### 示例：
```html
<body>
    <p contextmenu="supermenu">本段落拥有一个名为 "supermenu" 的上下文菜单。这个菜单会在用户右键单击该段落时出现。</p>
    <menu id="supermenu">
        <command label="Step 1: Write Tutorial" onclick="doSomething()">
        <command label="Step 2: Edit Tutorial" onclick="doSomethingElse()">
    </menu>
    <p><b>注释：</b>目前只有 Firefox 支持 contextmenu 属性。</p>
</body>
```

> ### 支持：
* 不支持的元素：无
* 支持的浏览器：Firefox

## draggable 属性 ※
> ### 说明：
* draggable 属性规定元素是否可拖动
* 链接和图像默认是可拖动的
* true值，表示元素可拖动
* false值，表示元素不可拖动
* auto值，表示浏览器自动判断元素是否可拖动

> ### 示例：
```html
<head>
    <style type="text/css">
        #div1 {width:350px;height:70px;padding:10px;border:1px solid #aaaaaa;}
    </style>
    <script>
    function allowDrop(ev){
        ev.preventDefault();
    }
    function drag(ev){
        ev.dataTransfer.setData("Text",ev.target.id);
    }
    function drop(ev){
        var data=ev.dataTransfer.getData("Text");
        ev.target.appendChild(document.getElementById(data));
        ev.preventDefault();
    }
    </script>
</head>
<body>
    <div id="div1" ondrop="drop(event)" ondragover="allowDrop(event)"></div>
    <br />
    <p id="drag1" draggable="true" ondragstart="drag(event)">这是一段可移动的段落。请把该段落拖入上面的矩形。</p>
</body>
```

> ### 支持：
* 不支持的元素：无
* 不支持的浏览器：IE9 -

## dropzone 属性 ※
> ### 说明：
* 规定在拖动被拖动数据时是否进行复制、移动或链接

> ### 有效值：
* 1

## hidden 属性 ※
> ### 说明：
* 规定元素仍未或不再相关

> ### 有效值：
* 1

## spellcheck 属性 ※
> ### 说明：
* 规定是否对元素进行拼写和语法检查

> ### 有效值：
* 1

## translate 属性 ※
> ### 说明：
* 规定是否应该翻译元素内容

> ### 有效值：
* 1

## irrelevant 属性 ※
> ### 说明：
* 设置元素是否相关。不显示非相关的元素

> ### 有效值：
* true
* false

## ref 属性 ※
> ### 说明：
* 引用另一个文档或本文档上另一个位置
* 仅在 template 属性设置时使用

> ### 有效值：
* url
* elementID

## registrationmark 属性 ※
> ### 说明：
* 为元素设置拍照
* 可规定于任何 <rule> 元素的后代元素，除了 <nest> 元素

> ### 有效值：
* registration mark

## template 属性 ※
> ### 说明：
* 引用应该应用到该元素的另一个文档或本文档上另一个位置

> ### 有效值：
* url
* elementID

## data-(*) 属性 ※
> ### 说明：
* data-* 属性用于存储页面或应用程序的私有自定义数据
* data-* 属性赋予我们在所有 HTML 元素上嵌入自定义 data 属性的能力

> ### 示例：
```html
<body>
    <ul>
        <li data-animal-type="bird">Owl</li>
        <li data-animal-type="fish">Salmon</li>
        <li data-animal-type="spider">Tarantula</li>
    </ul>
</body>
```

> ### 支持：
* 不支持的元素：无
* 不支持的浏览器：IE9 -
