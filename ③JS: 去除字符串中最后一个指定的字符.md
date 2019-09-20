#### 去除字符串中最后一个指定的字符  
```javascript
function filterCode(str, ele){
  let lastIndex = str.lastIndexOf(ele);
  if(lastIndex !== -1){
    var arr = str.split('');
    arr.splice(lastIndex,ele.length);
    var newstr = arr.join('')
    console.log(newstr)
  }
}

filterCode('helllo', 'l')
filterCode(' ha l d dd', 'd')
filterCode('vavava','va')
```

