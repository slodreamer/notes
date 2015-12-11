#快速绘制一个三角形
>如何使用border属性最快速的创建一个三角形
```html
  <div class="trangle"></div>
```
```css
.trangle {
    width:0;
    height:0;
    line-height:0;
    border:10px solid transparent;
    border-right-width:0;
    border-left-color:#f00;
  }
```

＃绘制锐角三角形
```html
  <div class="a"></div>
```
```css
  a:before {
  content: "";
  height: 0;
  width: 0;
  line-height: 0;
  border: 300px solid transparent;
  border-left-width: 0;
  border-right-color: #f90;
  border-width: 300px 1120px;
  position: absolute;
  top: 0;
  left: 0;
  }
  a:after {
  content: "";
  height: 0;
  width: 0;
  line-height: 0;
  border: 300px solid transparent;
  border-left-width: 0;
  border-right-color: #fff;
  border-width: 300px 1120px;
  position: absolute;
  top: 1;
  left: 0;
  }
```


