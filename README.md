# reverse-string
利用回调完成字符串的逆转 
```javascript
function reverse(str){
  if(str.length === 1){
    return str;
  }
  var s = str.substr(str.length-1,1);//截取字符串的最后一个
  var newStr = str.substring(0,str.length-1);//获取去掉最后一个字符的字符串
  return s + reverse(newStr);
}
```
