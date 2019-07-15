### [html]: 页面导入样式时， 使用 link 和 @import 有什么区别？    
###### 1. @import语法：  
```  
@import url; // url是一个表示要引入资源位置的<string>或者<uri>。这个url可以是绝对路径或者是相对路径。
@inport url list-of-media-queries; // list-of-media-querues 是一个逗号分隔的媒体查询条件列表，决定url引入的css规则在什么条件下应用。
```  
###### 2. 区别（参考网址：https://blog.csdn.net/u013778905/article/details/52885924 https://juejin.im/post/5ab36d99f265da23866fccd1 ）  
2.1  link 属于XHTML标签，除了加载CSS之外，还可以定义RSS等其他事务；@important 属于CSS范畴，只能加载CSS；  
2.2 link引入css时，在页面载入时同时加载；而@important需要网页完全载入以后加载。所以会出现一开始没有css样式，闪烁一下出现样式的页面(网速慢的情况下);  
2.3 link 是XHTML标签，无兼容问题；@important是在CSS2.1提出的，IE5以下的浏览器不支持；  
2.4 link支持使用JavaScript控制DOM去改变样式；而@important不支持；
  
###### 涉及知识点：  
1. URI 和 URL 的区别：
URI: Uniform Resource Identifier，统一资源标识符  
URL: Uniform Resource Location, 统一资源定位符  
URI 在于 I，即Identifier ，是统一资源标识符，可以唯一标识一个资源；URL 在于 Locater ，一般来说（URL）统一资源定位符，可以提供找到该资源的路径，但URL 又是URI，因为它可以标识一个资源，所以URL是URI 的子集。通俗地讲，URL类型于家庭住址，URI 类似于身份证号码。参考地址：https://www.zhihu.com/question/21950864  
2. XHTML 和 HTML 的区别：  
XHTML元素必须被正确地嵌套;  
XHTML 元素必须被关闭；  
标签名必须用小写；  
XHTML 文档必须拥有根元素；
参考网站： https://www.jianshu.com/p/8e65f98980bb

