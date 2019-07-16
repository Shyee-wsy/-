### 圣杯布局  
###### 1. 原理：center的宽是100%，通过父元素的内边距padding，以及左右两边的负边距实现三列式布局；  
###### 2. 实现  
```html
<body>
  <div class="header">header</div>
  <div class="body">
    <div class="center">圣杯-中间</div>
    <div class="left">圣杯-左边</div>
    <div class="right">圣杯-右边</div>
  </div>
  <div class="footer">footer</div>
</body>
```

```css
.header, .footer{
  width: 100%;
  height: 30px;
  background: #666;
}
*{
  border: 1px solid ;
  box-sizing: border-box;
  text-align: center;
}
.body{
  background-color: white;
  width: 100%;
  height: 100px;
  padding: 0 180px;
}
.center{
  float: left;
  width: 100%;
  height: 100px;
  background: green;
}
.left{
  float: left;
  width: 180px;
  height: 100px;
   background: #0c9;
  position: relative;
  left: -180px;
  margin-left:-100%;
}
.right{
  float: right;
  width: 180px;
  height: 100px;
  background: #0c9;
  position: relative;
  right: -180px;
  margin-left: -100%;
}
```
### 双飞翼布局  
###### 1. 原理： 直接给中间的部分外边距margin
###### 2. 实现   
```html
<body>
  <div class="header">header</div>
  <div class="center">
    <div class="inside">双飞翼-中间</div>
  </div>
  <div class="left">双飞翼-左边</div>
  <div class="right">双飞翼-右边</div>
  
  <div class="footer">footer</div>
</body>
```
```css
.header{
  width: 100%;
  height: 30px;
  background: #666;
}
*{
  border: 1px solid ;
  box-sizing: border-box;
  text-align: center;
}
.center{
  float: left;
  width: 100%;
  height: 100px;
  background:green;
}
.left{
  float: left;
  width: 180px;
  height: 100px;
  margin-left: -100%;
  background:#0c9;
}
.right{
  float:left;
  width:200px;
  height: 100px;
  margin-left: -200px;
  background: #0c9;
}
.inside{
  margin: 0 200px 0 180px;
  height: 100px;
}
.footer{
  clear: both;
  width: 100%;
  height: 30px;
  background: #666;
}
```
