# 目录  
  #### 居中元素固定框和高  
<ol>
<li>absolute + 负maragin  
<li>absolute + calc
<li>absolute + margin auto
</ol>  

#### 居中元素不固定框和高
<ol>
<li>absolute + transform</li>
<li>lineheight</li>
<li>writing-mode</li>
<li>table</li>
<li>css-table</li>
<li>flex</li>
<li>grid</li>
</ol> 
    
 # 代码详解  
 ## 固定框和高  
公共代码  
html    
```html
<div class="wp">
  <div class="box size">123</div>
</div>
```  
```css
.size{
  width: 100px;
  height: 100px;
}
.box{
  background-color: pink;
}
.wp{
  border: 2px solid red;
  width: 300px;
  height: 300px;
}
```

#### 1. absolute + 负maragin
```css
.wp{
  position: relative;
}
.box{
  position: absolute; /* 绝对定位是基于子元素的左上角做变化；所以top:50% 就是左上角距离父元素左上角150px*/
  top: 50%; /*那么加上元素的高度100px，则元素距离父元素下边界只有50px了,所以下面margin-top向上移动50px。此处可以使用calc()直接计算出来，详情看下面一种方法*/
  left: 50%;
  margin-left: -50px; 
  margin-top: -50px; /* margin-bottom: 50px;是无效的*/
}
``` 
#### 2. absolute + calc()
```css
.wp{
  position: relative;
}
.box{
  position: absolute;
  top: calc(50% - 50px);
  left: calc(50% - 50px);
}
/*此方法依赖calc()的兼容性
```
  
#### 3. absolute + margin auto  
  ```css
.wp{
  position: relative;
}
.box{
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  margin: auto;
}
/*amzing! unbelievable!~ ~*/
```
  
## 无需固定框高    
### 公共代码  
html  
```html
<div class="wp">
  <div class="box">123</div>
</div>
```    
css
```css
.box{
  background-color: pink;
}
.wp{
  border: 2px solid red;
  width: 300px;
  height: 300px;
}
```  

#### 1. absolute + transform   
```css
.wp{
  position: relative;
}
.box{
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  /*translate(x,y)，2D平移*/
}
/*此方法依赖translate2D的兼容性*/
```

#### 2. line-height  
```css
.wp{
  line-height: 300px;
  text-align: center; /*设置水平居中*/
  font-size: 0px;
}
.box{
  font-size: 16px;
  display: inline-block;
  vertical-align: middle;
  line-height: initial;
  text-align:left;
}
```



      
参考地址：https://yanhaijing.com/css/2018/01/17/horizontal-vertical-center/
