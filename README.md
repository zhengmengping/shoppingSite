# shoppingSite
一个简单的购物网站，包括首页和详情页

# 下图是首页的效果图
![图片](https://github.com/zhengmengping/shoppingSite/blob/master/animation.gif)

# 下面是详情页的效果图
![图片](https://github.com/zhengmengping/shoppingSite/blob/master/animation1.gif)

# 放大镜效果
如果要亲手实现这个效果，或许并不是件容易的事情。不过，可以借助于插件，插件也是jQuery的特色之一。
此处采用的是名为jqzoom的插件。首先把它引入到页面中，代码如下：
`<script src="scripts/jquery.jqzoom.js" type="text/javascript"></script>`
查看官方网站的API使用说明，可以使用如下代码调用jqzomm：
```
$(function(){
	$('.jqzoom').jqzoom({
		zoomType: 'standard',
		len:true,
		preloadImages:false,
		alwaysOn:flase,
		zoomWidth: 340,
		zoomHeight: 340,
		xOffset: 10,
		yOffset: 0,
		position: 'right'
	});
 });
  ```
 将上面代码放入名为use_jqzooom.js的文件里，然后引入即可。
 
 # 产品图层遮罩层效果
 使用名为thickbox的插件。先引入jquery和css文件。
 ```
 <script src="scripts/jquery.thickbox.js" type="text/javascript"></script>
 <link rel="stylesheet" href="styles/thickbox.css" type="text/css">
 ```
 然后为需要应用该效果的超链接元素添加class="thickbox"和title属性。
