## 作用域的不同  
1. var声明的变量只能是全局作用域或者函数作用域；  
2. let允许声明变量在块级作用域中；    
``` javascript
for(var i = 0; i < 4; i++) {
  console.log(i);
}
output: 
0
1
2
3

for(let i = 0; i < 4; i++) {
  console.log(i);
}
output: 
0
1
2
3


for(var i = 0; i<4; i++){
  setTimeout(function() {  // 同步注册回调函数到异步的宏任务队列。
    console.log(i);        // 执行此代码时，同步代码for循环已经执行完成
  }, 0);
}
output:
4
4
4
4

for(let i = 0; i<4; i++){
  setTimeout(function() {  // 同步注册回调函数到异步的宏任务队列。
    console.log(i);        // 执行此代码时，同步代码for循环已经执行完成
  }, 0);
}
output:
0
1
2
3

var:
在for循环中加入定时器之后，由于定时器有延迟，虽然设置的时间是0，但是还是会延迟一段时间，所以此时的执行流程是：for循环正常执行，
跳过定时器，当定时器开始执行的时候，for循环已经执行结束，开始打印i。而var定义变量的作用域是全局或者函数作用域，所以此时i始终
指向同一个值，所以最后打印的是i最后的结果。最后一次执行完i为3，i++后i为4。  

let：
let定义的变量作用域为块级作用域，每次执行完该模块的代码后，变量被销毁，所以在模块外面访问不了该变量。
每执行一次for循环，都会产生一个新的块级作用域，并且产生一个新的i，内部的函数是可以访问外部函数的变量的，所以定时器可以访问到
外部的i。每次setTimeout都要打印一个i，并将i销毁，外部的for循环要等待定时器销毁i，并执行i++，生成新的i完成下一次循环，所以
输出的结果打印了i的变化。
```


## 重复声明  
1. var 允许重复声明;  
2. let 不允许重复声明；  
``` javascript  
if(x){
  let foo;
  let foo; // SyntaxError thrown;  
}  
```
## 暂存死区  
1. var在声明但未初始化之前访问变量不会报错，返回undefined；  
2. let 在变量初始化之前访问变量会导致ReferenError；  
``` javascript  
function do_something(){
  console.log(bar); //undefined
  console.log(foo); //ReferenError
  var baar = 1;
  var foo = 2;
}
