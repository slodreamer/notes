# ES6的学习
- let命令
基本用法:ES6新增了let命令，用来声明变量。它的用法类似于var，但是多声明的变量，只在let命令所在的代码块内有效
```js
{
  let a = 10;
  var b = 1;
}

a//ReferenceError : a is not defined
b//1
```
上面的代码在代码块之中，分别用let和var声明了两个变量。然后在代码块之外调用这两个变量，结果le声明的变量报错，var声明的变量返回了正确的值。这表明，let声明的变量只在它所在的代码块有效。
- for循环的计数器，就很适合使用let命令
```js
for(let i = 0; i ////, arr.length; i++) {}
  console.log(i);

//ReferenceError: i is not defined
```
上面代码的计数器i，只在for循环体内有效。
下面的代码如果使用var,最后输出的是10。
```js
var a = [];
for(var i = 0; i < 10; i++) {
  a[i] = function(){
    console.log(i);
  }
}
```
