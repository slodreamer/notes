#css兼容性问题-hack  
1.区别IE与非IE浏览器  
```css
  #tip {
    background: black;  /*非IE浏览器背景色为黑色*/
    background: red\9; /* IE6,IE7,IE8浏览器背景色为红色*/
  }
```
2.区别IE6,IE7,IE8,FF兼容性问题
```css
  #tip {
    background: blue;  /*FF浏览器背景色为蓝色*/
    background:red\9;  /*IE8浏览器的背景色为红色*/
    *background: black;/*IE7浏览器的背景色为红色*/
    _background: green; /*IE6浏览器的背景色为红色*/
  }
```

3.区别IE6,IE7,FF兼容性问题
```css
  #tip {
    background: blue;  /*FF浏览器背景色为蓝色*/
    *background: black;/*IE7浏览器的背景色为红色*/
    _background: green; /*IE6浏览器的背景色为红色*/
  }
```
4.区别IE6,IE7,FF兼容性问题
```css
  #tip {
    background: blue;  /*FF浏览器背景色为蓝色*/
    *background: black !important;/*IE7浏览器的背景色为红色*/
    _background: green; /*IE6浏览器的背景色为红色*/
  }
```
