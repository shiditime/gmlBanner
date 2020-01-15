- $(".banner") 这是调用插件的对象为轮播图的父级框
- banner() 轮播图插件函数，接收两个参数
+ 第一个参数要切换图片的集合，必填
- 第二个参数是轮播图的轮播方式属性，选填，有默认规则
    + but:true,    // 左右按钮默认为true
    + butahidden:true,    // 是否自动隐藏左右按钮默认隐藏
    + list:true,  // 导航按钮
    + index:3,    //初始从第几个开始默认为0
    + autoPlay:true,  // 自动轮播默认为true
    + delayTiem:2000,  // 延迟时间默认为2000
    + moveTime:500    // 远动时间默认为300
```css

.box{height:300px;width:1000px;margin: 0 auto;position: relative;}
.imgbox img{height:300px;width:1000px}
```
```html
<div class="banner box">
    <div class="imgbox">
        <img src="images/1.jpg" alt="">
        <img src="images/2.jpg" alt="">
        <img src="images/3.jpg" alt="">
        <img src="images/4.jpg" alt="">
        <img src="images/5.jpg" alt="">
    </div>
</div>
<div class="banner1 box">
    <div class="imgbox">
        <img src="images/1.jpg" alt="">
        <img src="images/2.jpg" alt="">
        <img src="images/3.jpg" alt="">
        <img src="images/4.jpg" alt="">
        <img src="images/5.jpg" alt="">
    </div>
</div>
```
```js

$(".banner").banner($(".banner").find("img"),{
    but:false,    // 左右按钮默认为true
    butahidden:true,    // 是否自动隐藏左右按钮默认隐藏
    list:false,  // 导航按钮
    index:3,    //初始从第几个开始默认为0
    autoPlay:true,  // 自动轮播默认为true
    delayTiem:2000,  // 延迟时间默认为2000
    moveTime:500    // 远动时间默认为300
});
$(".banner1").banner($(".banner1").find("img"));


```

