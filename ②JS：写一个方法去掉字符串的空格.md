#### 写一个方法去掉字符串的空格  
###### 相关知识点  

1. <b>trim()方法：</b> 用于去掉字符串首尾的空格，该方法不会改变原始字符串；  

2. <b>for...in 语句:</b> 以任意顺序遍历一个对象的除Symbol以外的可枚举属性；(遍历属性）  
MDN：https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Statements/for...in  

3. <b>for...of 语句:</b> 在可迭代对象（包括Array，Map，Set，String, TypeArray, arguments对象等等）上创建一个迭代循环，调用自定义迭代钩子，  
并为每个不同属性的值执行语句（遍历值）  
MDN: https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Statements/for...of  
  
4. <b>forEach():</b> 该方法对数组的每个元素执行一次提供的函数；  
MDN：https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach  
  
5. <b>正则表达式</b>  
（1） var express = / pattern / flags;  
模式（pattern）部分可以是任何简单或复杂的正则表达式，可以包含字符类、限定符、分组、向前查找以及反向引用；标志（flags）用以表明正则表达式的行为，可以是  
g、i和m 的任意组合。g（global）表示全局模式，即模式将被应用于所有字符串，而非在发现第一个匹配项时立即停止；i表示不区分大小写；m（multiline）表示多行  
模式，即在到达一行文本末尾时还会继续查找下一行中是否存在与模式匹配的项；  
元字符 \s 表示匹配一个空白字符，包括空格、制表符、换行符合换页符。+ ： 表示匹配前一个表达式1次或者多次，等价于{1,}  
正则表达式方法replace(): 一个在字符串中测试匹配的string方法，并且使用替换字符串替换掉匹配到的子字符串。
###### 使用正则表达式实现  
```javascript
function test(str){
 str1 = str.replace(/\s+/g,'');
  console.log(str1)
}
```
