#### Ducument类型
> JavaScript通过Document类型表示文档，在浏览器中，document对象是HTMLDocument的一个实例，表示整个HTML页面。而且，document对象是window对象的一个属性，因此可以作为全局对象来访问。

##### Document节点特征   
1. `nodeType`值为`9`  
2. `nodeName`值为`"document"`
3. `nodeValue`值为`null`
4. `parentNode`值为`null`
5. `ownerDocument`值为`null`  

##### HTMLDocument:
`HTMLDocument`属性:  
1. `title` //修改浏览器标题栏`document.title`  
2. `URL` //完整`URL`  
3. `domain` //域名  
4. `referrer` //来源页面的URL

`HTMLDocument`方法:  
1. `namedItem(name)`,可以通过元素的name特性取得集合中项
```html
  <img src="image.png" name="image">
```
```javascript
  var image = document.getElementsByTagName("img").namedItem("image");
```
2. `item(index)`,可以通过索引值取得集合中项
```html
  var image = images["image"];
  // 同 var image = images.item(0);
```
