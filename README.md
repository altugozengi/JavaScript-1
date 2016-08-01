# JavaScript
JavaScript诞生于1995年，由Netscape Navigator公司开发。
一个完整的JavaScript实现应该由三个部分组成：核心（ECMAScript）、文档对象模型（DOM）、浏览器对象模型（BOM）。

ECMAScript：由ECMA－262定，提供核心语言功能。ECMAScript与Web浏览器没有依赖关系，实际上这门语言本身并不包含输入和输出定义，它只是定义了这门语言的基础，在此基础上可以构建更完善的脚本语言。
我们常见的Web浏览器只是ECMAScript实现可能的宿主环境之一，宿主环境不仅提供基本的EMCAScript实现，同时也会提供该语言的扩展，以便语言与环境之间对接交互。而这些扩展，如：DOM，则是利用ECMAScript的核心类型和语法提供更多的具体功能。
ECMAScript主要规定了这门语言的下列部分：语法、类型、语句、关键字、保留字、操作符和对象。

文档对象模型（DOM）：是针对XML但经过扩展用语HTML的应用程序编程接口（API）。
DOM把整个页面映射为一个多层节点结构，通过这个DOM结构，开发人员获得控制页面内容和结构的主动权。借助DOM提供的API，开发人员可以轻松自如的实现增删改查节点操作。
DOM级别：DOM1、DOM2和DOM3。

DOM1于1998年10月成为W3C推荐标准。DOM1级由两个模块组成：DOM核心（DOM Core）和DOM HTML。其中DOM Core映射XML的文档结构，以便简化对文档中任意部分的访问和操作。DOM HTML模块则在DOM核心的基础上加以扩展，添加了针对HTML的对象和方法［DOM并不只是针对JavaScript的，很多别的语言也都实现了DOM，只是在Web浏览器中，基于ECMAScript实现的DOM已经成为JavaScript这门语言的重要组成部分］。
如果说DOM1级目标是映射文档结构的，那么DOM2级目标要宽泛多了。DOM2级引入了新模块：DOM视图（DOM Views）［定义了追踪不同文档，如：应用CSS之前和之后的文档的视图接口］、DOM事件（DOM Events）［定义了事件和事件处理接口］、DOM样式（DOM Style）［定义了基于CSS为元素应用样式的接口］、DOM遍历和范围（DOM Traversal and Range）［定义了遍历和操作文档树的接口］。
DOM3级进一步扩展了DOM，引入了统一方式加载和保存文档的方法，新增验证文档的方法。DOM3级也对DOM核心进行了扩展，开始支持XML1.0规范［DOM0级只是DOM历史上一个参照点，具体来说是指Internet Explorer4.0和Netscape Navigator4.0最初支持的DOM］。

浏览器对象模型（BOM）：访问和控制浏览器窗口的浏览器对象模型。开发人员使用BOM可以控制浏览器显示的页面以外的部分。
而BOM真正与众不同的地方，还是它作为JavaScript实现的一部分但却没有相关的标准。这个问题在HTML5中得到解决。从根本上讲，BOM只处理浏览器窗口和框架；但人们习惯也把针对JavaScript扩展算作BOM的一部分。如：弹出新浏览器窗口、移动缩放和关闭浏览器窗口、提供navigator，location，screen对象、对cookies的支持等。
