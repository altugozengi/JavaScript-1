### Element类型
#### 特征
1. `nodeType`值为1  
2. `nodeName`值为标签名  //`tagName`返回和`nodeName`相同，`tagName`容易理解而已【都是大写的标签名】
3. `nodeValue`值为`null`  

#### HTML元素
`HTML`元素都是由`HTMLElement`类型表示，`HTMLElement`除了继承自`Element`并添加了一些属性。  
1. `id`，元素在文档中的唯一标识  
2. `title`，有关元素的附加信息  
3. `className`，与元素`class`对应  
例如：
```javascript
<div id="myDiv" class="bd" title="body"></div>
<script>
var dir = document.getElementById('myDiv');
alert(dir.id); // "myDiv"
alert(dir.className); // "bd"
alert(dir.title); // "body"
// 可以利用该属性更改元素属性
div.id = "yourDiv";
div.className = "yd";
div.title = "footer";
</script>
```
#### 取得特性
操作特性的`DOM`方法有三个：`getAttribute()`、`setAttribute()`和`removeAttribute()`