#快速绘制一个三角形
>如何使用border属性最快速的创建一个三角形
、、、html
<div class="caret"></div>
、、、
、、、css
  .caret {
    width:0;
    height:0;
    line-height:0;
    border:10px solid transparent;
    border-right-width:0;
    border-left-color:#f00;
  }
、、、


