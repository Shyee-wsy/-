##### 描述：简述下CSS3有哪些新增的特性？如：
圆角：border-radius: 3px  
css参考手册： http://www.w3school.com.cn/cssref/index.asp#table  
### CSS3 动画属性  
```
@keyframes: 规定动画
animation: 所有动画的简写属性，除了 animate-paly-state 属性；
animate-name: 规定@keyframes 动画的名称；
animate-duration: 规定动画完成一个周期所花费的秒或毫秒；
animate-duration: 规定动画完成一个周期所花费的秒或毫秒； 
animation-timing-function: 规定动画的速度曲线；
animation-delay: 规定动画何时开始；
animation-iteration-count: 规定动画是否在下一周期逆向地播放；
animation-direction: 规定动画是否在下一周期逆向地播放；
animation-play-state: 规定动画是否正在运行或者暂停；
animation-fill-mode: 规定对象动画之外的状态；
```
### CSS 背景属性  
```
background-clip: 规定背景的绘制区域；
background-origin: 规定背景图片的定位区域；
background-size: 规定背景图片的尺寸；
``` 
### CSS 边框属性
```
border-bottom-left-radius: 定义边框左下角的形状；
border-bottom-right-radius: 定义边框右下角的形状；
border-image: 简写属性，设置所有border-image-* 属性
border-image-outset: 规定边框图像区域超出边框的量；
border-image-repeat: 图像边框是否应平铺（repeated）、铺满（rounded）或拉伸（stretched）；
border-image-slice: 规定图像边框的内向偏移；
border-image-source: 规定用作边框的图片；
border-image-width: 规定图片边框的高度；
border-radius: 简写属性，设置所有四个border-*-radius 属性；
border-top-left-radius: 定义边框左上角的形状；
border-top-right-radius: 定义边框右下角的形状；
box-shadow: 向方框添加一个或多个阴影；
```
### Box属性
```
overflow-x: 如果内容溢出了元素内容区域，是否对内容的左/右边缘进行裁剪；
overflow-y: 如果内容溢出了元素内容区域，是否对内容的上/下边缘进行裁剪；
overflow-style: 规定溢出元素的首选滚动方式；
rotation: 围绕由 rotation-point 属性定义的点进行旋转；
rotation-point: 定义距离上左边框边缘的偏移点；
```
### Color属性
``` 
color-profile: 允许使用源的颜色配置文件的默认以外的规范；
opacity: 规定元素的不透明级别;
rendering-intent: 允许使用颜色配置文件渲染意图的默认以外的规范；
```
### 可伸缩框属性（Flexible Box）
```
box-align: 规定如何对齐框的子元素；
box-direction: 规定框的子元素的显示方向；
box-flex: 规定框的子元素是否可伸缩；
box-flex-group: 将可伸缩元素分配到柔性分组；
box-lines: 规定当超出父元素框的空间时，是否换行显示；
box-ordinal-group: 规定框的子元素的显示次序；
box-orient: 规定框的子元素是否应水平或者垂直排列；
box-pack: 规定水平框中的水平位置或者垂直框中的垂直位置；
```
### Grid属性
```
grid-columns: 规定网格中每个列的宽度；
grid-rows: 规定网格中每个列的高度；
```
### Hyperlink属性
```
target: 简写属性，设置target-name、target-new 以及target-position属性；
target-name: 规定在何处打开链接（链接的目标）；
target-new: 规定目标链接在新窗口还是在已有窗口的新标签页中打开；
target-position: 规定在何处放置新的目标链接；
```
### Marquee属性
``` 
marquee-direction: 设置移动内容的方向；
margin-play-count: 设置内容移动多少次；
margin-speed: 设置内容滚动得多快;
margin-style: 设置移动内容的样式;
```
### 多列属性（Multi-column）
```
column-count: 规定元素应该被分割的列数；
column-fill: 如何填充列；
column-gap: 列之间的间隔；
column-rule: 设置所有column-rule-* 属性的简写属性；
column-rule-color: 规定列之间规则的颜色；
column-rule-style: 规定列之间规则的样式；
column-rule-width: 规定列之间规则的宽度；
column-span: 规定元素应该横跨的列数；
column-width: 规定列的宽度；
coLumns: 规定设置 column-width 和 column-count 的简写属性；
```
### Paged Media 属性
```
fit: 示意如何对 width 和 height 属性均不是 auto 的被替换元素进行缩放；
fit-positon: 定义盒内对象的对齐方式；
image-orientation: 规定用户代理应用于图像的顺时针方向旋转；
page: 规定元素应该被显示的页面特定类型；
size: 规定页面内容包含框的尺寸和方向；
```
### CSS文本属性（Text）
```
hanging-punctuation: 规定标点字符是否位于线框之外；
punctuation-trim: 规定是否对标点字符进行修剪；
text-align-last: 设置如何对齐最后一行或紧挨着强制换行符之前的行；
text-emphasis: 向元素的文本应用重点标记以及重点标记的前景色；
text-justify: 规定当 text-align 设置为 "justify" 时所使用的对齐方式；
text-outline: 规定文本的轮廓；
text-overflow: 规定当文本溢出包含元素时发生的事情；
text-shadow: 向文本添加阴影；
text-wrap: 规定文本的换行规则；
word-break: 规定非中日韩文本的换行规则；
word-wrap: 允许对长的不可分割的单词进行分割并换行到下一行；
``` 
### 2D/3D 转换属性（Transform）
```
transfrom: 向元素应用 2D 或 3D 转换；
transform-origin: 允许你改变被转换元素的位置；
transform-style: 规定被嵌套元素如何在 3D 空间中展示；
perspective: 规定 3D 元素的透视效果；
perspective-origin: 规定 3D 元素的底部位置；
backface-visibility: 定义元素在不面对屏幕时否可见；
```
### 过渡属性（Transition）
```
transition: 简写属性，用于在一个属性中设置四个过渡属性；
transition-property: 规定应用过渡的CSS属性的名称；
transition-duration: 定义过渡效果花费的时间；
transition-timing-function: 规定过渡效果的时间曲线；
transition-delay: 规定过渡效果何时开始；
```
### 用户界面属性（User-interface）
```
appearance: 允许您将元色设置为标准用户界面元素的外观；
box-sizing: 允许您以确切的方式适应某个区域的具体内容；
icon: 为创作者提供使用图表化等价物来设置元素样式的功能；
nav-down: 规定在使用 arrow-down 导航键时向何处导航；
nav-index:设置元素的 tab 键控制次序；
nav-left: 规定在使用 arrow-left 导航键时向何处导航；
nav-right: 规定在使用 arrow-right 导航键时向何处导航；
nav-up: 规定在使用 arrow-up 导航键时向何处导航；
outline-offset: 对轮廓进行偏移，并在超出边框边缘的位置绘制轮廓；
resize: 规定是否可由用户对元素的尺寸进行调整；
```
