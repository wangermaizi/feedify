#### 1. 文件的引用
```html
<script src="js/jquery.min.js"></script>
<script src="js/feedify.min.js"></script>      
```

#### 2. html结构设置
```html
<div class="feedify">
  <div class="feedify-item">
   <div class="feedify-item-header">
    This is the header of my item.
    It will remain stuck to top while scrolling.
   </div>
   <div class="feedify-item-body">
    This is the body of my item.
    I can put whatever I want in here.
   </div>
  </div>
</div>   
```
#### 3. css的样式设置
```css
.feedify .feedify-item {
  position: relative;
}
.feedify .feedify-item .feedify-item-header {
  z-index: 100;
}
.feedify .feedify-item.fixed .feedify-item-header {
  position: fixed;
  top: 0;
}
.feedify .feedify-item.bottom .feedify-item-header {
  position: absolute;
  bottom: 0;
}     
```

#### 4. 插件调用
```js
$(function() {
  $('.feedify').feedify();
});   
```

#### 5. 备注
Feedify的主题使用的是Bootstrap。
如果使用它，你要在页面中引入Bootstrap3.3.4+版本的Bootstrap文件。

```html
<link href="http://maxcdn.bootstrapcdn.com/bootstrap/3.3.4/css/bootstrap.min.css" rel="stylesheet">
<link href="css/feedify.min.css" rel="stylesheet">
<link href="css/feedify-theme.min.css" rel="stylesheet">   
```
