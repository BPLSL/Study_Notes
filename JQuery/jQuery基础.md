### 使用JQuery的步骤

1. 引入jQuery：

```javascript
// 方法一：通过本地的jQuery库引用
<script src="jquery-1.10.2.min.js"></script>
// 方法二：通过 CDN（内容分发网络）引用，常用的有Staticfile CDN、百度、又拍云、新浪、谷歌和微软的服务器都存有 jQuery 。
<script src="http://libs.baidu.com/jquery/1.10.2/jquery.min.js">
```

2. 使用jQuery选择器定位节点
3. 使用jQuery方法操作节点





### jQuery选择器



#### 元素选择器

jQuery通过元素名来选取元素

例如：选取页面中的所有<P>

``` javascript
var p = $("p")
```



#### id选择器---使用"#"

选择id为total的元素

``` javascript
$("#total")
```



#### class选择器---使用"."

选择class为total的元素

```javascript
$(".total")
```



#### 组合选择器

选择