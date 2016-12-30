## javascript 原生DOM

> 光标锁定input输入框

```javascript
 window.onload = function() {
                var inputFocus = document.getElementByTagName('input');
                console.info(inputFocus);
                for (var i=0; i < inputFocus.length; i++) {
                    if (inputFocus[i].type == 'text') {

                        inputFocus[i].focus();
                        break;
                    }
                }
            }
```
> 设置title值 
```javascript
document.setTitle = function(t) {
  document.title = t;
  var i = document.createElement('iframe');
  i.src = '//m.baidu.com/favicon.ico';
  i.style.display = 'none';
  i.onload = function() {
    setTimeout(function(){
      i.remove();
    }, 9)
  }
  document.body.appendChild(i);
}
```
> 正则表达式
```javascript
用户名 "^[a-zA-Z]\\w{5,17}$";
密码*/ "^[a-zA-Z0-9]{6,16}$";
手机号 /^1(3[0-9]|4[57]|5[0-35-9]|7[0135678]|8[0-9])\d{8}$/
"^((13[0-9])|(15[^4,\\D])|(17[0-9])|(18[0-9]))\\d{8}$";
邮箱*/ "^([a-z0-9A-Z]+[-|\\.]?)+[a-z0-9A-Z]@([a-z0-9A-Z]+(-[a-z0-9A-Z]+)?\\.)+[a-zA-Z]{2,}$";
汉字 "^[\u4e00-\u9fa5],{0,}$";
身份证 "(^\\d{18}$)|(^\\d{15}$)";
IP地址  "(25[0-5]|2[0-4]\\d|[0-1]\\d{2}|[1-9]?\\d)";
```